Release: ChimeraOS v45-Pre-Release2-Asus-Rog-Ally Hotfix
![image](https://github.com/lm209/CLD1610/assets/82281970/af8a5528-fa7b-4735-882b-7803c66b1ecc)
ASUS ROG ALLY
-

![image](https://github.com/lm209/CLD1610/assets/82281970/fe080242-bee1-4ff4-870b-9d87be351d50)
ARRIVES TO
-

![image](https://github.com/lm209/CLD1610/assets/82281970/14965267-248c-43e3-a8b2-1735896209b1)
CHIMERAOS=STEAMOS
-



-------------------------------------------------------------------------
ENGLISH USER GUIDE# 
ChimeraOS Asus Rog Ally Setting Up
-------------------------------------------------------------------------
ITS RECOMMENDED TO HAVE THE BIOS AND MCU FIRMWARE UP TO DATE!
PLEASE UPDATE BEFORE, OVER MYASUS OR THE OFFICIAL DRIVER & SUPPORT SITE!
-------------------------------------------------------------------------
Note: This operating system is still under development.  There could be errors and missing components.  However, the operating system is in a stable state
-------------------------------------------------------------------------

1.

Download the latest Release Package and Extract it

Create a Windows 11 ISO with the "Media Creation Tool"

Create a bootable USB Drive with "Rufus"

Boot it up, Format and delete all Partitions

Leave the Partition to unallocated

Make a force Shutdown (hold the power button until it shutdown)

Go to the bios and "Disable Secure Boot under "Security" Options.

Make with "Etcher" a bootable USB Drive with the ChimeraOS ISO

Boot it up

Connect to Wifi or Ethernet in the Setup

Select the SSD to install ChimeraOS

Select the "Advanced User Installation" and Install the "Unstable Build"

-------------------------------------------------------------------------
2.

After installation, Login to your Steam Account 

Now go to the Desktop mode and Open the Console Application.

Password is "gamer"

type in:

sudo frzr-unlock

curl -L https://github.com/SteamDeckHomebrew/decky-loader/raw/main/dist/install_release.sh | sh

curl https://raw.githubusercontent.com/CryoByte33/steam-deck-utilities/main/install.sh | bash -s --

Start Cryoutilities and change all to Recommended, reboot now

-------------------------------------------------------------------------

3.

Install the Official PowerTools Plugin from Decky Loader

Extract the "PowerTools.zip" to the "Downloads" Folder

Open the Console and Type:

sudo systemctl stop plugin_loader

rm ~/.config/powertools/*.json

rm $HOME/.config/powertools/limits_cache.json

sudo cp --preserve=mode /home/gamer/Downloads/backend $HOME/homebrew/plugins/PowerTools/bin/backend

sudo cp --preserve=mode /home/gamer/Downloads/index.js $HOME/homebrew/plugins/PowerTools/dist/index.js

sudo systemctl start plugin_loader

sudo reboot

-------------------------------------------------------------------------

4.

Adding Fan Curve Setting with Console:

sudo pacman -S base-devel

pikaur -S rog-control-center

Open Rog Control Center

Setting up your Curve Profiles and save it in the GUI

sudo systemctl start asusd

sudo reboot

If you Update rog-control-center then Type this:

systemctl daemon-reload

systemctl restart asusd

-------------------------------------------------------------------------

5.

Activate VRR in the Steam Menu

Download Wine Cellar from Decky Loader, to Download the latest Proton


-------------------------------------------------------------------------









GERMAN USER GUIDE#
ChimeraOS Asus Rog Ally Anleitung 
-------------------------------------------------------------------------
ES WIRD EMPFOHLEN, DAS BIOS UND DIE MCU-FIRMWARE AUF DEM AKTUELLSTEN STAND ZU HABEN!  BITTE VORHER AKTUALISIEREN, ÜBER DIE MYASUS APP ODER DIE OFFIZIELLE TREIBER UND SUPPORT-SEITE!
-------------------------------------------------------------------------
Hinweis: Dieses Betriebssystem befindet sich noch in der Entwicklung.  Es kann zu Fehlern und fehlenden Komponenten kommen.  Das Betriebssystem befindet sich jedoch in einem stabilen Zustand
-------------------------------------------------------------------------

1.

Ladet euch das letzte Release Package herunter

Erstellt mit den "Media Creation Tool" eine Windows 11 ISO

Benutzt nun "Rufus" um einen bootbaren USB Stick zu erstellen

Booten Sie über den USB Stick und formatieren und löschen Sie alle Partitionen.

Lassen Sie die Partition auf "nicht zugewiesen"

Führen Sie ein erzwungenes Herunterfahren durch (halten Sie den Netzschalter gedrückt, bis er herunterfährt).

Gehen Sie zum BIOS und deaktivieren Sie „Sicheres Booten“ unter „Security“-Optionen.

Benutzt nun das Programm "Etcher" um einen bootbaren USB Stick mit der ChimeraOS ISO zu erstellen 

Bootet nun über den USB Stick 

Stellen Sie im Setup eine Verbindung zu WLAN oder Ethernet her

Wählen Sie die SSD aus, um ChimeraOS zu installieren

Wählen Sie die „Advanced User Installation“ und installieren Sie „Unstable Build“.

-------------------------------------------------------------------------

2.

Richtet nun Steam mit euren Account ein

Gehen Sie nun in den Desktop-Modus, drückt unten rechts auf den Menü Button, dort auf den X-Gnome Ordner und öffnen Sie die Konsolenanwendung.

Passwort ist „gamer“

Befolgt nun diese Befehle:

sudo frzr-unlock

curl -L https://github.com/SteamDeckHomebrew/decky-loader/raw/main/dist/install_release.sh | sh

curl https://raw.githubusercontent.com/CryoByte33/steam-deck-utilities/main/install.sh | bash -s --

Startet nun Cryoutilities, PW ist "gamer" und wählt recommended Setting aus. Startet danach das Gerät neu.

-------------------------------------------------------------------------

3.

Installiert das offizielle PowerTools Plugin aus dem Decky Loader und öffnet den Desktop Modus 

Extrahiert die "PowerTools.zip" in den Ordner „Downloads“.

Öffnen Sie die Konsole und geben Sie Folgendes ein:

sudo systemctl stop plugin_loader

rm ~/.config/powertools/*.json

rm $HOME/.config/powertools/limits_cache.json

sudo cp --preserve=mode /home/gamer/Downloads/backend $HOME/homebrew/plugins/PowerTools/bin/backend

sudo cp --preserve=mode /home/gamer/Downloads/index.js $HOME/homebrew/plugins/PowerTools/dist/index.js

sudo systemctl start plugin_loader

sudo reboot

-------------------------------------------------------------------------

4.

Lüfterkurven einstellen mit folgenden Befehl:

sudo pacman -S base-devel

pikaur -S rog-control-center

Öffnet das Rog Control Center

Stellet eure Lüfterkurven in der GUI ein und speichert diese ab

Danach:

sudo systemctl start asusd

sudo reboot

Sobald ihr dem Rog Control Center ein Update verpasst gibt folgendes ein:

systemctl daemon-reload

systemctl restart asusd

-------------------------------------------------------------------------

5.

Aktivieren Sie VRR im Steam-Menü

Laden Sie das Wine Cellar Plugin von Decky Loader herunter, um das aktuellste Proton zu installieren 

