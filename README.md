# 
ChimeraOS Asus Rog Ally Setting Up

ITS RECOMMENDED TO HAVE THE BIOS AND MCU FIRMWARE UP TO DATE!
PLEASE UPDATE BEFORE, OVER MYASUS OR THE OFFICIAL DRIVER & SUPPORT SITE!

1.

Download the Windows Media Creation Tool and create a bootable USB Drive: https://www.microsoft.com/de-de/software-download/windows11 (not needed if you Download my Release)

Boot it up, Format and delete all Partitions

Leave the Partition to unallocated

Make a force Shutdown (hold the power button until it shutdown)

Go to the bios and "Disable Secure Boot under "Boot" Options.

Download this Build here: https://github.com/kzkzkzkzkzk/install-media/releases/tag/2023-09-05_81a7337 (not needed if you Download my Release)

Download Etcher and make a bootable USB Drive: https://etcher.balena.io/ (not needed if you Download my Release)


Boot it up

Connect to Wifi or Ethernet in the Setup

Select the SSD to install ChimeraOS

Select the "Advanced User Installation" and Install the "Unstable Build

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

Again to Console Application:
 
sudo pacman -S python-setuptools

sudo systemctl stop handycon

pikaur -Sy handygccs-git

type first "Y" and the second "N"

sudo systemctl enable --now handycon

sudo reboot

##############################################

4.

Again:

systemctl --user disable chimera

sudo reboot

###########################################

5.
 
To enable refresh rate changing on these devices, enable developer mode in steam and check the "Enable refresh rate changing with external displays" option.

###########################################

6.

Install Official PowerTools from Decky Loader Store

Download this two files for modded Version: https://github.com/hicder/PowerTools/releases/tag/v2.1 (not needed if you Download my Release)

Extract these two files to the "Downloads" Folder

Open the Console and Type:

sudo systemctl stop plugin_loader

rm ~/.config/powertools/*.json

rm $HOME/.config/powertools/limits_cache.json

sudo cp --preserve=mode /home/gamer/Downloads/backend $HOME/homebrew/plugins/PowerTools/bin/backend

sudo cp --preserve=mode /home/gamer/Downloads/index.js $HOME/homebrew/plugins/PowerTools/dist/index.js

sudo systemctl start plugin_loader

sudo reboot

##############################################

7.

Activate VRR in the Steam Menu and Change the Hz Refresh to 120hz.

Download ProtonUp-Qt from the Discovery Store or use Wine Cellar from Decky Loader 

Download the latest GE Proton!!!

Now you are done. ChimeraOS should be working perfectly. If you Update the System, you are not need to Set Up ChimeraOS again.
