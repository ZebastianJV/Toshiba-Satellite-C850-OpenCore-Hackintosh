# Toshiba-Satellite-C850-OpenCore-Hackintosh
Welcome to the repository of my hackintosh build. This is a prebuilt for the laptop that ive been always using for OpenCore.

# Model used:
Toshiba Satellite C850-B990

# Specs i have
	CPU:Intel Core i3-3120M
	GPU:Intel HD Graphics 4000
	RAM:8GB DDR3 SODIMM 1333Mhz
	HDD:200GB TOSHIBA HDD 5400 RPM
# IMPORTANT:
	This prebuilt Hackintosh is not 100% guarenteed to work as it might vary, its all about luck.
	This only works on Ivy Bridge CPUS and will not work with Satellite C850s with NVIDIA Discrete GPU.
	The CPU Must be Intel Core i3/i5/i7-3XXXM
	MAKE SURE TO BACKUP YOUR DATA AS THIS ERASES YOUR WHOLE DISK.

# What works:
	Ethernet 10/100Mbps
	Battery
	Graphics Acceleration (Intel HD Graphics 4000 1536MB VRAM)
	AC Charger
	Internal WebCam
	WebCam light
	HDMI

# What doesnt work (so far):
	Sound is not working cause i am dumb using AppleALC so i just use a soundcard.
	External Monitors through VGA
	Internal Trackpad
	Microphone jack (prob needs AppleALC)
	Internal Microphone
	Function Keys even with external keyboard (this might vary)

# What i havent tested yet (Untested)
	Internal Keyboard
	
	
# Keep in note
That if you have a really cheap mechanical feel keyboard like i do, people that uses scroll lock to have the LEDs on wont work cause of macOS not supporting scroll lock or numlock.
If you wanna change brightness sometimes the keyboard button for scroll lock is brightness down and pause break is brightness up for some reason but at least they used some of the more usesless keys.

# Steps that ive used
1. Click Download source code as zip in this repository.
2. Extract the zip file
3. Copy the EFI Folder from there
4. Plug in your USB Drive (at least 4GB)
5. And drag the EFI Folder there
6. Once Done, you should have OpenCore Bootloader working now all you need to is follow the OpenCore Guide to show how to get the recovery image and get it on the drive. https://dortania.github.io/OpenCore-Install-Guide/installer-guide/
7. Once done with getting the recovery image restart your laptop and press F2 on Toshiba Logo.
8. Make sure you have these options enabled
	Boot Option: UEFI
	Fast Boot: Disabled
	Secure Boot: Disabled
9. Once done with tweaking the BIOS Settings, press F10 and Save And Exit.
10. This time press F12 and boot into your drive that you plugged in.
11. Boot to your External Drive (dmg) and hit enter
12. Once booted in after Apple Logo, you will be presented to a macOS Recovery. Just accept all the terms.
13. Now go to Disk Utility and Click View and click Show All Devices/Drives.
14. Erase your Drive and Change the Partition name to whatever you want. (in my case Macintosh HD)
15. Erase it as GUID Partition Map and APFS Format.
16. Once Done, close Disk Utility and Then Click Reinstall and then accept the terms. (make sure your connected to internet via ethernet)
17. And Choose your Partition and wait until it installs.
18. It will take a long time depending on your internet as macOS is very big. (Big Sur for example is 12GB)
19. Now once it rebooted, go back and boot to your usb by pressing f12.
20. Now this time choose macOS Installer and make sure you chose the one in the right drive and not the USB Drive.
21. Wait another 30 minutes or more for it to be done.
22. Once rebooted, boot into your USB again and choose macOS Installer again.
23. Once it rebooted again, one more time boot into your USB Drive and this time boot into the partition that you formatted earlier. (in my case Macintosh HD)
24. Now proceed with the setup and after that, your pretty much done.
25. If you made it this far. Congratulations you succesfully installed macOS. But theres a few more things we need to do.
# Boot into macOS without USB
Now this time you installed macOS, but you cant boot to it without your usb as you dont have a bootloader on your internal drive yet so this time.
1. In macOS
Mount your EFI. (There are several methods but you can use either Clover Configurator or MountEFI. Its up to you) https://github.com/corpnewt/MountEFI
2. Now Copy the EFI Folder from your USB Drive and paste it in your EFI Partition. If it asks that you want to replace the folder, then click yes.
3. Now Reboot, and now you have bootloader without USB Drive.
4. Done. You successfully installed macOS and OpenCore bootloader.
