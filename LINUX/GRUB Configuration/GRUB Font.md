To increase the font size of the GRUB menu on an Arch Linux system, follow these steps:

*For my system 15" laptop with `1920x1080` resolution screen `font size 24` worked well*

*On an Arch system running `JakooLit's Hyprland` configuration, `FiraCode-Regular` was the font that I used.*
### 1. **Generate a Larger Font**

GRUB uses `pf2` font files, and you can generate a larger one using `grub-mkfont`:

`sudo grub-mkfont -s 32 -o /boot/grub/fonts/DejaVuSansMono32.pf2  /usr/share/fonts/TTF/DejaVuSansMono.ttf`

- Replace `32` with your desired font size.
- You can also use other fonts from `/usr/share/fonts/TTF/`.

### 2. **Configure GRUB to Use the New Font**

Edit the GRUB configuration file:

`sudo nano /etc/default/grub`

Add (or modify) the GRUB_FONT variable:

`GRUB_FONT="/boot/grub/fonts/DejaVuSansMono32.pf2"`

*I had to add this variable to my GRUB configuration*

### 3. **Update GRUB Configuration**

Run the following command to apply the changes:

`sudo grub-mkconfig -o /boot/grub/grub.cfg`

### 4. **Reboot and Check**

Reboot your system and check if the font size has increased:

sudo reboot

If the font size is too small, try increasing the value in step 1 (e.g. `-s 40`)