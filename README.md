# 
ChimeraOS Asus Rog Ally Setting Up


0. Download the Windows Media Creation Tool and create a bootable USB Stick: https://www.microsoft.com/de-de/software-download/windows11
1. Boot it up format and delete all partitions
2. leave the Partition to unallocated
3. make a force shutdown
4. Download this build here: https://github.com/kzkzkzkzkzk/install-media/releases/tag/2023-09-05_81a7337
Download Etcher and make a bootable usb stick
boot it up
connect to wifi or Ethernet in the setup
select the ssd to install ChimeraOS
select the advanced user Installation and install the unstable build

Now go to the Desktop mode and Open the Console Application.
Password is "gamer"
type in:
sudo frzr-unlock
curl -L https://github.com/SteamDeckHomebrew/decky-loader/raw/main/dist/install_release.sh | sh
curl https://raw.githubusercontent.com/CryoByte33/steam-deck-utilities/main/install.sh | bash -s --
Start Cryoutilities and change all to Recommended, reboot now

 Again to Console Application
 sudo systemctl stop steam-patch
 curl -L https://github.com/Maclay74/steam-patch/releases/latest/download/install.sh | sh
 sudo reboot
 
5.2. sudo pacman -S python-setuptools
5.5. sudo systemctl stop handycon
5.6. pikaur -Sy handygccs-git
5.7. sudo systemctl enable --now handycon
5.8. sudo reboot
5.9. (If you have Double Inputs, then you must disable and enable handycon):
sudo systemctl disable handycon
sudo systemctl enable handycon
sudo reboot

6. systemctl --user enable chimera.service
6.1. sudo systemctl enable chimera-proxy.service
6.2. sudo systemctl enable chimera-proxy.socket
6.2.1. sudo reboot
6.3. systemctl --user enable steam-patch
6.3.1. sudo systemctl start steam-patch
6.3.2. sudo systemctl daemon-reload
6.3.3. sudo systemctl enable steam-patch.service
6.3.4. sudo systemctl start steam-patch.service
6.4. sudo reboot
7.1. systemctl --user disable chimera
7.2. sudo reboot
   
8. To enable refresh rate changing on these devices, enable developer mode in steam and check the "Enable refresh rate changing with external displays" option.

8.1. Install Official PowerTools from Decky Loader Store
Download this modded Version: https://github.com/hicder/PowerTools/releases/tag/v2.1
8.3. Open the Console and Type:
sudo systemctl stop plugin_loader
rm ~/.config/powertools/*.json
rm $HOME/.config/powertools/limits_cache.json
sudo cp --preserve=mode /home/gamer/Downloads/backend $HOME/homebrew/plugins/PowerTools/bin/backend
sudo cp --preserve=mode /home/gamer/Downloads/index.js $HOME/homebrew/plugins/PowerTools/dist/index.js
sudo systemctl start plugin_loader
sudo reboot
--------------------------------
NOT RECOMMEND YET!!! 8.4 Adding Fan Curve Setting with Console:
sudo pacman -S base-devel
sudo reboot
pikaur -S asusctl
sudo reboot
pikaur -S rog-control-center
sudo reboot
Open The Control Center and set up the Fans 
Add Control Center to Steam
(If this not working to have Control Center try:
pikaur -S paru-git
sudo reboot
paru -S asusctl
sudo reboot 
paru -S rog-control-center 
sudo reboot
Now you should have the Control Center)!!!
--------------------------------
9. Activate VRR in the Steam Menu and Change the Hz Refresh to 120hz.
10. Download ProtonUp-Qt
10.1. Download the latest GE Proton!!!
Now you are done. ChimeraOS should be working perfectly. If you Update the System, you are not need to Set Up ChimeraOS again.
