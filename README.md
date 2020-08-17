# thinkpad-t440s-efi-folder-osx-mojave
EFI folder for thinkpad t440s with clover bootloader

for hackintoshing a thinkpad t440s with osx mojave.
whats working:
graphic drivers
audio drivers
ethernet
usb
touchpad + gestures
keyboard shortcuts (for changing brightness & volume)
battery management
pretty much everything

what doesn't work:
wifi & bluetooth (intel wifi is not supported, fixed it with a wifi dongle)
camera (havent found a kext to get the camera working)

to install:

1. open terminal
2. paste sudo mkdir /Volumes/EFI into terminal
3. paste sudo mount -t msdos /dev/disk0s1 /Volumes/efi into terminal
4. open efi partition in finder
![Alt text](EFI.png?raw=true "Screenshot")
5. delete the content of the efi folder and paste my folder inside
![Alt text](EFI_delete.png?raw=true "Screenshot")
6. reboot and ur done :)
