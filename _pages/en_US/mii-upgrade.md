---
title: Mii Channel upgrade
---
{% include toc title="Table of Contents" %}

## Preface

While at first glance the Mii Channel may look the same as the one that came with previous models of the Wii, the Wii mini version is missing some features. You cannot share Miis by copying them over to Wii remotes, DSi consoles, or by sending them in the Mii Parade.
This is a result of Nintendo's attempts to reduce possible entrypoints to the console, as well as caused by a lack of online connectivity.
However, you can restore the full-fledged Mii channel by downloading it directly from Nintendo's servers.

## Instructions

### Section I - Installing Sharpii

To be able to download Wii software from the NUS servers, you will need a computer and a special app. If you are using Windows, [NUS Downloader](https://wiibrew.org/wiki/NUS_Downloader) is the easiest to use, please skip directly to Section II instead.
For macOS and Linux-based systems, Sharpii NetCore is the easiest option, but it requires use of a Terminal. Continue below.

1. Download the latest release of Sharpii NetCore from [TheShadowEevee's GitHub](https://github.com/TheShadowEevee/Sharpii-NetCore/releases/latest) for your operating system and architecture. 
	- If your machine has an Intel or AMD cpu, choose the x64 build for your Operating System. 
	- If using an Apple Silicon Mac, choose the MacOSX-arm64 build. 
	- If using an arm-based Linux box, choose the arm or arm64 build depending on the architecture.
1. Decompress the 7z and optionally copy the Sharpii executable to a location of your choice
1. (macOS/Linux only): Open your Terminal app (on macOS it's in the Utilities folder in your Launchpad), type `chmod +x ` and drag the Sharpii binary you just extracted from your file explorer to the terminal window, then hit enter to make it executable.
1. Open a terminal window in the folder Sharpii is in (or cd to it)
	- For Windows, while inside the folder in File Explorer, hit `Ctrl+L`, type `cmd` and hit `Enter`.
	- For macOS, go one directory above the folder, `Ctrl+Click` the folder icon > services > New Terminal at Folder

### Section II - Installing the WAD

1. 
	- For Windows, extract and run NUS Downloader, go to **Database... > System > 0010002484157XX - Mii Channel > 41 (All/System) > Latest Version**. Then untick all options from the bottom, tick **Pack WAD**, type `Mii-Channel.wad` and click on **Start NUS Download!**. 
		The WAD will be in a subfolder called titles inside the folder you extracted nusd to.
	- For macOS/Linux, while in the directory Sharpii is located in, copy and paste the following:
		```
		./Sharpii nusd -wad -id 0001000248414341 -o Mii-Channel.wad
		```
		The WAD will be saved to the same folder the Sharpii binary is in.

1. Copy the wad file to your Wii mini USB drive.
1. Follow the [Wii Mod Lite guide](https://wii.guide/wiimodlite) to install Mii-Channel.wad
1. Press home and return to the Wii Menu, launch the Mii Channel and you should now have everything available.

[Return to Pick-a-Pimp](pick-a-pimp) | [Continue to site navigation](site-navigation)<br>
We have other tutorials that you might like.
{: .notice--info}