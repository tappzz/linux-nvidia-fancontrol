# Step 1. Fix _Unable to open X config file '/etc/X11/xorg.conf' for writing_ error 
> sudo chmod +x /usr/share/screen-resolution-extra/nvidia-polkit
# Step 2 Configuring Xwrapper.config file
## Open Xwrapper.config file by typing
 > sudo vi /etc/X11/Xwrapper.config
## Before _allowed_users=console_ add the following line: 
 > needs_root_rights=yes
## *On Fedora Linux, you may have to add both of these lines:
 > needs_root_rights=yes

 > allowed_users=console

Write-out and save the file. Reboot your PC.


# Step 3. Coolbits-4 installation
 > sudo nvidia-xconfig --cool-bits=4
# Step 4. GreenWithEnvy installation
 > flatpak --user install flathub com.leinardi.gwe





Thanks to

[Galang Hanafi](https://github.com/galanghanaf/fix-manual-fan-control-nvidia-linux) 

[Roberto Leinardi ](https://gitlab.com/leinardi/gwe)
