# thinkpad-t440s-efi-folder-osx-mojave
EFI folder for thinkpad t440s with clover bootloader

for hackintoshing a thinkpad t440s with osx mojave.
whats working:
1. graphic drivers
2. audio drivers
3. ethernet
4. usb
5. touchpad + gestures
6. keyboard shortcuts (for changing brightness & volume)
7. battery management
8. pretty much everything

what doesn't work:
1. wifi & bluetooth (intel wifi is not supported, fixed it with a wifi dongle)
2. camera (havent found a kext to get the camera working)

to install:

1. open terminal
2. paste sudo mkdir /Volumes/EFI into terminal
3. paste sudo mount -t msdos /dev/disk0s1 /Volumes/efi into terminal
4. open efi partition in finder
![Alt text](pics/EFI.png?raw=true "Screenshot")
5. delete the content of the efi folder and paste my folder inside
![Alt text](pics/EFI_delete.png?raw=true "Screenshot")
6. reboot and ur done :)
