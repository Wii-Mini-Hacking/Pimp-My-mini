---
title: Pick-a-Pimp
---
{% include toc title="Table of Contents" %}
## Possible upgrades

Thanks to the hard work done by the Wii mini Hacking community members, many features of the original Wii have been brought back to the Wii mini, either through software or hardware means, or a mix of both.
Specifically:

- Homebrew execution was brought to the console via the [Bluebomb](https://github.com/Fullmetal5/bluebomb) exploit back in 2019 by Fullmetal5. (instructions on [wii.guide](https://wii.guide/bluebomb))
- Game backups through USB loaders can be played using Leseratte's custom d2xl cIOS, built on top of the d2x cIOS for the original Wii (see above link)
- You can replace the stripped down Mii Channel with the full version by downloading it from Nintendo's servers using Sharpii or NUSD (see guide below)
- Wired internet connectivity can be restored through Fullmetal5's [Ethernet Enabler Homebrew](https://wiibrew.org/wiki/Ethernet_Enabler) and using any off-the-shelf USB LAN adapter that utilises the AX88772 network chip¹. We have found that this adapter from UGREEN appears to work fine: [Amazon Europe](https://www.amazon.de/dp/B00MYT481C) [Amazon US](https://www.amazon.com/dp/B08DRKYKMM/)
- All the WiFi circuits are available on the board, however some components, the adapter connector and the wifi card itself are missing. You can get all the required parts as [a kit from webhdx's Tindie store](https://www.tindie.com/products/webhdx/wifi-kit-for-wii-mini/)
- A reset switch can be restored either by simply soldering a reset button or using webhdx's [sdrst kit](https://www.tindie.com/products/webhdx/wiimini-sdrst-sd-reset-button-mod-for-wii-mini/) (see guides below)
- An SD/microSD card reader can be restored by soldering any SD/microSD card adapter to the test points on the board, or more easily by using webhdx's [sdrst kit](https://www.tindie.com/products/webhdx/wiimini-sdrst-sd-reset-button-mod-for-wii-mini/) (see guides below)
- Component (YPbPr) Video (and thus 480p output) is available from the console's Audio-Video Encoder (AVE) chip but is not electrically connected to the AV Multi out port of the console to save space and money. However, the [miniRGBii](https://github.com/Wii-Mini-Hacking/miniRGBii) mod designed by Job, Devnol and other contributors from the Wii mini Hacking discord can restore the missing filtering circuitry for component video to properly function.
- Gamecube controller ports 1 and 4, as well as Memory Card port 1 have available test pads on the board and can be immediately restored. Ports 2 and 3 are present but lack safety circuits and thus should not be used. This mod should be plug-and-play in either Wii games that support GC controllers (such as Mariokart Wii), or GC games through Nintendont. Playing original GameCube minidiscs is not supported on the Wii mini.

(1) While connection to the Internet will be available, use of services such as WiiConnect/RiiConnect24 or Nintendo WFC/wiimmfi are not available without the installation of a WiFi card and an original Wii System menu along with original IOS.
## Available Guides

The following guides are currently available, with more to come in the future:

<!--- TBA: [webhdx\'s SDRST add-in board for a reset button and microSD card slot](sdrst)-->
- [Reset Switch](reset)
- [Generic SD/microSD Card Slot](sdcard)
- [miniRGBii add-in board for component video/480p output](miniRGBii)
<!--- TBA: [WiFi Adapter install](wifi)-->
<!--- TBA: [GameCube controller ports 1&4](gcc)-->
<!--- TBA: [GameCube memory card slot 1](gcmem)-->
- [Mii Channel restore removed features](mii-upgrade)
