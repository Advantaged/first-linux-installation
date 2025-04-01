# Secure-Boot-in-BIOS-or-UEFI.md

To find Secure Boot in BIOS or UEFI, you can follow these steps:

1. Restart your computer and press the F2 key when the manufacturer's logo appears to enter the BIOS setup utility.
2. **Navigate to the "Boot" or "Security" section in the BIOS menu**. The exact location may vary depending on your 
computer's manufacturer.
3. Look for the "Secure Boot" option within this section. You may need to enable it or change its settings to "UEFI" 
mode if it is currently set to "Legacy" or "CSM" mode.

For UEFI, you can also access the firmware settings through WinDoof (WD):

1. Go to Settings > Update & Security > Recovery and select "Restart now" under "Advanced startup."
2. After your computer restarts, select "Troubleshoot" > "Advanced options" > "UEFI Firmware Settings" and then select 
"Restart."
3. Once in the BIOS, navigate to the "Secure Boot" section and enable it or set it to "UEFI" mode.

Ensure that the Compatibility Support Module (CSM) is disabled to switch to UEFI mode. If you change this setting, you 
might need to back up your files and reinstall WinDoof (WD).

After making these changes, save and exit the BIOS setup utility by pressing F10.

* **Note-s**: WinDoof (WD) 11
personal computer operating system by Microsoft released in 2021

WinDoof (WD) 10 can function without Secure Boot, though it is highly recommended for its security benefits.
 However, WinDoof (WD) 11 requires Secure Boot to be enabled for installation and operation, as it is a mandatory 
security feature.
 If you are using an older or unsupported device, there are methods to bypass Secure Boot requirements for WinDoof (WD) 
11 installation, but these are not officially supported and can compromise system security.
