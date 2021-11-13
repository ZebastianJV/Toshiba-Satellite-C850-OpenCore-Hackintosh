# Toshiba-Satellite-C850-OpenCore-Hackintosh
Welcome to the repository of my hackintosh build. This is a prebuilt for the laptop that ive been always using for OpenCore.
IMPORTANT:
This prebuilt Hackintosh is not 100% guarenteed to work as it might vary, its all about luck.
This only works on Ivy Bridge CPUS and will not work with Satellite C850s with NVIDIA Discrete GPU.
The CPU Must be Intel Core i3/i5/i7-3XXXM

# What works:
	Ethernet 10/100Mbps
	Battery
	Graphics Acceleration (Intel HD Graphics 4000 1536MB VRAM)
	AC Charger
	Internal WebCam
	WebCam light

# What doesnt work (so far):
	Sound is not working cause i am dumb using AppleALC so i just use a soundcard.
	External Monitors through VGA
	Internal Trackpad
	Microphone jack (prob needs AppleALC)
	Internal Microphone
	Function Keys even with external keyboard (this might vary)

# What i havent tested yet (Untested)
	Internal Keyboard
	HDMI
	
# Keep in note
That if you have a really cheap mechanical feel keyboard like i do, people that uses scroll lock to have the LEDs on wont work cause of macOS notsupporting scroll lock or numlock.
If you wanna change brightness sometimes the keyboard button for scroll lock is brightness down and pause break is brightness up for some reason but at least they used some of the more usesless keys.

# Steps that ive used
1. Click Download source code as zip in this repository.
2. Extract the zip file
3. Copy the EFI Folder from there
4. Plug in your USB Drive (at least 4GB)
5. And drag the EFI Folder there
6. Once Done, you should have OpenCore Bootloader working now all you need to is follow the OpenCore Guide to show how to get the recovery image and get it on the drive. https://dortania.github.io/OpenCore-Install-Guide/installer-guide/

