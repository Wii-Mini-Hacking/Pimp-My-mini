---
title: SD Card
---
{% include toc title="Table of Contents" %}
<!--If you're looking for a more elegant solution to this and the SD card mod, [WebHDX's sd-rst board](sdrst) is for you.
{: .notice--info }-->

An SD card slot is a helpful addition to the Wii mini, as it enables the use of some homebrew that do not work with a USB drive, such as BootMii IOS for creating NAND backups, it also allows you to have a lower profile storage medium than a USB device.

## Parts Required

1. 	An SD or microSD card breakout board that supports the SD protocol (not just SPI) We recommend [this SD card reader from Sparkfun](https://www.sparkfun.com/products/12941) or [this push-push microSD one from Adafruit](https://www.adafruit.com/product/4682) (Not affiliated with either company)
1.	Multiple colours of thin (≤32awg) wire, 7-8 colours are recommended for easier wiring, you may also use a wire ribbon for the same effect.
1.	An SD or microSD card of your choice, formatted as fat32 with Master Boot Record. (While any size should work, some homebrew will not work with cards above 32gb and a few older ones may even have a 2gb limit)
1.	(Optional) A 10-100nF ceramic capacitor of any kind for decoupling

## Installation

1.	Cut 8 strands of wire of the same length (the shorter and the closer they are in length to each other, the better the signal integrity). They should start from the test point section marked [C] on the bottom side of the board (coloured blue in the picture below) and reach to where you want your SD card slot to be mounted. Make sure to give them a little extra slack to allow for stripping the ends and in case you make a mistake. It's easier if the wires are different colours so that you can tell them apart, or if you use ribboned wire.
	![Wii mini board bottom side](/Pimp-My-mini/images/motherboard/motherboard-side-a.png)
1.	Board section [C] contains the following test pads:

	![Section C TP numbering](/Pimp-My-mini/images/motherboard/SectionC-SDcard.png)

	these map to the following pins on the sd card adapters (they may have multiple names depending on your adapter):

	<button class="tablinks btn btn--large btn--primary" id="defaultOpen" onclick="openTab(event, 'SD')">SD</button>
	<button class="tablinks btn btn--large btn--info" onclick="openTab(event, 'microSD')">microSD</button>

	<div id="SD" class="blanktabcontent" markdown="1">
	| Test Pad | Name(s) | SDcard pin |
	|----------|---------|------------|
	|TP166     |Dat2     |9           |
	|TP167     |Dat3/CS  |1           |
	|TP163     |CMD/DI/MOSI   |2      |
	|TP172     |GND/VSS  |3,6         |
	|TP171     |3v3/VDD/Vin|4         |
	|TP162     |CLK      |5           |
	|TP164     |Dat0/DO/MISO  |7      |
	|TP165     |Dat1     |8           |
	|TP168     |CD/Det (Card Detect)|N/A, on breakout board|
	|TP169     |WP/WL (Write Lock)|N/A, on breakout board|
	
	(if CD and/or WL are unavailable, short TP168 and/or TP169 respectively to ground to bypass them).

	SD Card pins map as follows (image provided by [pinouts.org](https://pinouts.org)): ![SD Pinout](/Pimp-My-mini/images/SD-pinout.png)

	</div>

	<div id="microSD" class="blanktabcontent" markdown="1">
	| Test Pad | Name(s) | microSD card pin |
	|----------|---------|------------|
	|TP166     |Dat2     |1           |
	|TP167     |Dat3/CS  |2           |
	|TP163     |CMD/DI/MOSI   |3      |
	|TP171     |3v3/VDD/Vin|4         |
	|TP162     |CLK      |5           |
	|TP172     |GND/VSS  |6           |
	|TP164     |Dat0/DO/MISO  |7      |
	|TP165     |Dat1     |8           |
	|TP168     |CD/Det (Card Detect)|N/A, on breakout board|
	|TP169     |WP/WL (Write Lock)|N/A, wire it to any GND|
	
	(if CD is unavailable, short TP168 to any ground to bypass it).

	microSD Card pins map as follows (image provided by [pinouts.org](https://pinouts.org)): ![microSD Pinout](/Pimp-My-mini/images/microSD-pinout.png)

	</div>
1. You may optionally add a 10-100nF ceramic capacitor between 3.3v and gnd near the sd slot for decoupling.

## Post-Install

While the card reader is installed, it will not be functional yet, as the stock Wii mini IOS does not include SD support. For that, you will have to install a customized version of the original Wii IOS that removes the need for a WiFi card, as well as the original Wii system menu to restore the removed SD card menu.

<script>
	let tabcontent = document.getElementsByClassName("blanktabcontent");
    let tablinks = document.getElementsByClassName("tablinks");

    function openTab(evt, tabName) {
        let element;

        for (element of tabcontent) {
		element.style.display = "none";
        }

        for (element of tablinks) {
            element.className = element.className.replace("btn--primary", "btn--info");
            if (!element.className.includes('btn--info'))
                element.className += " btn--info";
        }

        document.getElementById(tabName).style.display = "block";
        evt.currentTarget.className = evt.currentTarget.className.replace("btn--info", "btn--primary");
    }

    // Get the element with id="defaultOpen" and click on it
    document.getElementById("defaultOpen").click();
</script>

[Continue to installing the System Menu (no WiFi card)](sminstall-nowifi)
Without a WiFi card, a special procedure has to be followed to restore SD card functionality, as well as other stripped out features.
{: .notice--info }

<!-- TODO: Add link to WiFi guide -->

We'd love to see your completed mod, feel free to join us on [our Discord](https://discord.gg/6ryxnkS) and post a picture in #pimping-general
{: .notice--success }