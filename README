## Installlation

**Using git:**  
<code>$ git clone git://github.com/Generator/Grub2-themes.git  
\# cp -r Grub2-themes/{Archlinux,Archxion} /boot/grub/themes/</code>

**Edit your /etc/default/grub and change line:**
<code>\#GRUB_THEME="/path/to/gfxtheme"  
to  
GRUB_THEME="/boot/grub/themes/Archxion/theme.txt"  
or  
GRUB_THEME="/boot/grub/themes/Archlinux/theme.txt"</code>

**The resolution the theme was designed to show best at 1024x768:**  
<code>GRUB_GFXMODE=auto  
to  
GRUB_GFXMODE=1024x768</code>  

**Update grub configuration:**  
<code>\# grub-mkconfig -o /boot/grub/grub.cfg</code>

**Archlinux AUR:**  
Soon...


## FAQ  

**My distribution does not have icon in boot menu, how can I add?**  
Find your distribution/OS class  
<code>\# grep 'menuentry' '--class' /boot/grub/grub.cfg</code>  
should be first after the name of the distribution/OS.  

E.g.: The class for ArchLinux is arch  
<code>menuentry 'Arch Linux' --class **arch** --class gnu-linux --class gnu --class os</code>  

Rename the image to the class name (arch.png)  
Resize the image to 32x32, and copy it to */boot/grub/themes/THEME/icons/*  
(Images must be in PNG)  

**Can I change the background or color of the theme?**  
Choose an image, converts and resizes to 1024x768 in PNG  
Copy the image to */boot/grub/themes/THEME/*  
Edit */boot/grub/themes/THEME/theme.txt*:  
<code>desktop-image: "background.png" # Theme background image  
desktop-color: "#000000" # Theme color</code>


**How can I change the logo theme**  
Copy your logo image to */boot/grub/themes/THEME/* (must be in PNG)  
Edit */boot/grub/themes/THEME/theme.txt*:  
<code>\+ image {  
id = "\__archlogo__"  
left = 30%  
width = 10%  
top = 2%  
height = 12%  
file = "archlogo.png" \# distribution logo</code>  


## References: 
[GNU GRUB Manual 1.99](http://www.gnu.org/software/grub/manual/grub.html#Theme-file-format)  
[GRUB Graphical Menus Project](http://grub.gibibit.com/Theme_format)  
[The Definitive Guide To Theming GRUB 2 v1.99](https://docs.google.com/open?id=0B82343FTJphIbElHUGVac1hBZnc)  


## Ideas or suggestions to share in: 
[Issues](https://github.com/Generator/Grub2-themes/issues)
[ArchLinux Forums](https://bbs.archlinux.org/viewtopic.php?id=141631)
[Twiter @American_Jesus](https://twitter.com/American_Jesus)

