# 
ChimeraOS Asus Rog Ally Setting Up

1.

Download the Windows Media Creation Tool and create a bootable USB Stick: https://www.microsoft.com/de-de/software-download/windows11

Boot it up format and delete all partitions

Leave the Partition to unallocated

Mke a force shutdown

Go to the bios and disable secure boot under boot options.

Download this build here: https://github.com/kzkzkzkzkzk/install-media/releases/tag/2023-09-05_81a7337

Download Etcher and make a bootable usb stick: https://etcher.balena.io/

boot it up

connect to wifi or Ethernet in the setup

select the ssd to install ChimeraOS

select the advanced user Installation and install the unstable build

##################################################

2.

Now go to the Desktop mode and Open the Console Application.

Password is "gamer"

type in:

sudo frzr-unlock

curl -L https://github.com/SteamDeckHomebrew/decky-loader/raw/main/dist/install_release.sh | sh

curl https://raw.githubusercontent.com/CryoByte33/steam-deck-utilities/main/install.sh | bash -s --

Start Cryoutilities and change all to Recommended, reboot now

###############################################

3.

Again to Console Application

sudo systemctl stop steam-patch

curl -L https://github.com/Maclay74/steam-patch/releases/latest/download/install.sh | sh

sudo reboot
 
sudo pacman -S python-setuptools

sudo systemctl stop handycon

pikaur -Sy handygccs-git

sudo systemctl enable --now handycon

sudo reboot

(If you have Double Inputs, then you must disable and enable handycon):

sudo systemctl disable handycon

sudo systemctl enable handycon

sudo reboot

##############################################

4.

systemctl --user enable chimera.service

sudo systemctl enable chimera-proxy.service

sudo systemctl enable chimera-proxy.socket

sudo reboot

systemctl --user enable steam-patch

sudo systemctl start steam-patch

sudo systemctl daemon-reload

sudo systemctl enable steam-patch.service

sudo systemctl start steam-patch.service

sudo reboot

systemctl --user disable chimera

sudo reboot

###########################################

5.
 
To enable refresh rate changing on these devices, enable developer mode in steam and check the "Enable refresh rate changing with external displays" option.

###########################################

6.

Install Official PowerTools from Decky Loader Store

Download this two files for modded Version: https://github.com/hicder/PowerTools/releases/tag/v2.1

Open the Console and Type:

sudo systemctl stop plugin_loader

rm ~/.config/powertools/*.json

rm $HOME/.config/powertools/limits_cache.json

sudo cp --preserve=mode /home/gamer/Downloads/backend $HOME/homebrew/plugins/PowerTools/bin/backend

sudo cp --preserve=mode /home/gamer/Downloads/index.js $HOME/homebrew/plugins/PowerTools/dist/index.js

sudo systemctl start plugin_loader

sudo reboot

############################################

7.

NOT RECOMMEND YET!!!

Adding Fan Curve Setting with Console:

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

(Now you should have the Control Center)!!!

##############################################

8.

Activate VRR in the Steam Menu and Change the Hz Refresh to 120hz.

Download ProtonUp-Qt or use Wine Cellar from Decky Loader 

Download the latest GE Proton!!!

Now you are done. ChimeraOS should be working perfectly. If you Update the System, you are not need to Set Up ChimeraOS again.
