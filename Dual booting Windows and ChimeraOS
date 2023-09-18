Dual booting Windows and ChimeraOS on the same Disk
Some considerations first:

1. This guide assumes you already have a fully functional installation of Windows 11 on the target disk, complete with a properly configured EFI partition.

2. This guide was made with the ROG Ally.

1. Enter the BIOS and disable Secure Boot:
Some users have encountered issues with this step. For example, on the ROG Ally, ASUS sometimes resets the value. To successfully disable it, I disabled Secure Boot, booted into Windows, unlocked the HD with a Bitlocker key obtained from the Microsoft website, and on the next boot, Secure Boot was successfully disabled.

2. Disable Bitlocker (if you have it disabled, skip this step)
In Windows settings, search for 'Bitlocker' or 'Encryption' and disable disk encryption. This process can take approximately one hour as it decrypts each file on the disk.

3. Prepare to Install ChimeraOS from a USB Stick
You can use Balena Etcher for this step.

4. Boot from the ChimeraOS USB Stick via BIOS
You should have another disk connected to the hub, either another USB drive or a micro SD card. This is because the system will not allow you to install ChimeraOS on the same disk as Windows without completely erasing it. Hence, we first install it onto an intermediate disk.

5. Shrink the Data Partition in Windows
There are multiple ways to do this; choose the method that works best for you. I used the Device Manager that comes bundled with Windows.

6. Migrate frzr_root partition to the internal drive
After installing ChimeraOS, migrate the big partition (frzr_root) to the internal NVMe drive using the space you freed in step 5. The duration of this process will be proportional to the size of the partition being migrated. For that step you can use a tool called "Macrium Reflect" that has a free trial.

7. Patch the EFI Folder
Manually merge the EFI partition created by the ChimeraOS installer with the one on the internal NVMe. If you installed rEFInd previously, there's no need to replace '/EFI/BOOT/BOOTX64.efi', as we will use the Systemd one to boot ChimeraOS.

8. Create a Boot Option in BIOS for ChimeraOS
In BIOS, go to advanced mode and to Bios tab, create a manual boot entry pointing to '/EFI/systemd/systemd-bootx64.efi' and name it 'ChimeraOS'. You can use this to boot directly.

9. Partition Labels Required by ChimeraOS
ChimeraOS expects to find two partitions by label:

10. frzr_root: This is where your system and home directories are located. If you cloned using the software mentioned above, the label will be automatically applied. If not apply it using e2label /dev/nvme0n1pX frzr_root (replace X with the right partition)
frzr_efi: This is the boot partition. You should rename it using fatlabel /dev/nvme0n1p1 frzr_efi.
Dual Boot Windows and ChimeraOS
At this point, you should be able to dual boot Windows and ChimeraOS and also apply OTA updates from ChimeraOS without affecting Windows. You can change the boot order in BIOS to choose the default system.

11. Bonus Step: Install rEFInd to Manage Dual Boot
Although it might seem redundant now (on the Ally, more information bellow), installing rEFInd could be very useful in the near future. Here are the steps:

Install rEFInd on the internal NVMe drive by following the instructions on the rEFInd page.

Configure rEFInd. There are many documents available to guide you, and the sample configuration file provided is comprehensive. Perhaps someone can provide examples at a later stage.

IMPORTANT: On the Ally, currently, the D-pad and touchscreen will only work in rEFInd if you boot manually from BIOS. We are hoping for a solution from ASUS to address this issue.
