ENGLISH USER GUIDE# 
ChimeraOS Asus Rog Ally Setting Up

ITS RECOMMENDED TO HAVE THE BIOS AND MCU FIRMWARE UP TO DATE!
PLEASE UPDATE BEFORE, OVER MYASUS OR THE OFFICIAL DRIVER & SUPPORT SITE!

Note: This operating system is still under development.  There could be errors and missing components.  However, the operating system is in a stable state

####################################################

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

#################################################

3. NOT available at the Moment!
 
To enable refresh rate changing on these devices, enable developer mode in steam and check the "Enable refresh rate changing with external displays" option.

#################################################

4.

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

5.

Activate VRR in the Steam Menu and Change the Hz Refresh to 120hz.

Download ProtonUp-Qt from the Discovery Store or use Wine Cellar from Decky Loader 

Download the latest GE Proton!!!

Now you are done. ChimeraOS should be working perfectly. If you Update the System, you are not need to Set Up ChimeraOS again.

###############################################









GERMAN USER GUIDE#
ChimeraOS Asus Rog Ally Anleitung 
-------------------------------------------------------------------------
ES WIRD EMPFOHLEN, DAS BIOS UND DIE MCU-FIRMWARE AUF DEM AKTUELLSTEN STAND ZU HABEN!  BITTE VORHER AKTUALISIEREN, ÜBER DIE MYASUS APP ODER DIE OFFIZIELLE TREIBER UND SUPPORT-SEITE!
-------------------------------------------------------------------------
Hinweis: Dieses Betriebssystem befindet sich noch in der Entwicklung.  Es kann zu Fehlern und fehlenden Komponenten kommen.  Das Betriebssystem befindet sich jedoch in einem stabilen Zustand
-------------------------------------------------------------------------

1.

Laden Sie das Windows Media Creation Tool herunter und erstellen Sie ein bootfähiges USB-Laufwerk: https://www.microsoft.code/software-download/windows11 (nicht erforderlich, sofern Sie mein Release herunterladen)

Booten Sie über den USB Stick und formatieren und löschen Sie alle Partitionen.

Lassen Sie die Partition auf "nicht zugeordnet"

Führen Sie ein erzwungenes Herunterfahren durch (halten Sie den Netzschalter gedrückt, bis er herunterfährt).

Gehen Sie zum BIOS und deaktivieren Sie „Sicheres Booten“ unter „Security“-Optionen.

Ladet euch diese Version herunter: https://github.com/kzkzkzkzkzk/install-media/releases/tag/2023-09-05_81a7337 (nicht erforderlich, sofern Sie mein Release herunterladen)

Booten nun über den USB Stick 

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

3. MOMENT NICHT ZUR VERFÜGUNG, WIR HABEN UNS DAZU ENTSCHLOSSEN ES VORÜBERGEHEND ZU DEAKTIVIEREN!

Um die Änderung der Bildwiederholfrequenz auf diesen Geräten zu aktivieren, aktivieren Sie den Entwicklermodus in Steam, geht auf Entwickler ganz unten in der Leiste und aktivieren Sie die Option „Änderung der Bildwiederholfrequenz mit externen Displays aktivieren“.

-------------------------------------------------------------------------

4.

Installiert das offizielle PowerTools aus dem Decky Loader Store herunter (nicht löschen)

Laden Sie diese beiden Dateien für die modifizierte Version herunter: https://github.com/hicder/PowerTools/releases/tag/v2.1 (nicht erforderlich, sofern Sie mein Release herunterladen)

Extrahieren Sie diese beiden Dateien in den Ordner „Downloads“.

Öffnen Sie die Konsole und geben Sie Folgendes ein:

sudo systemctl stop plugin_loader

rm ~/.config/powertools/*.json

rm $HOME/.config/powertools/limits_cache.json

sudo cp --preserve=mode /home/gamer/Downloads/backend $HOME/homebrew/plugins/PowerTools/bin/backend

sudo cp --preserve=mode /home/gamer/Downloads/index.js $HOME/homebrew/plugins/PowerTools/dist/index.js

sudo systemctl start plugin_loader

sudo reboot

-------------------------------------------------------------------------

5.

Aktivieren Sie VRR im Steam-Menü und ändern Sie die Hz-Aktualisierung auf 120 Hz.

Laden Sie ProtonUp-Qt aus dem Discovery Store herunter oder verwenden Sie Wine Cellar von Decky Loader

Laden Sie das neueste GE Proton herunter!!!

Jetzt sind Sie fertig. ChimeraOS sollte perfekt funktionieren. Wenn Sie das System aktualisieren, müssen Sie ChimeraOS nicht erneut einrichten.
