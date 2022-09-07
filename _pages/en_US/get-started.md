---
title: "Get Started"
---

{% include toc title="Table of Contents" %}

Let's get started with pimping your Wii mini.

### First of all, some ground rules

This guide is only intended for **advanced** users and requires the use of soldering equipment that can cause serious burns and damage to your console or even a fire if used improperly. Continue **AT YOUR OWN RISK**. You have been warned. None of the authors of this guide, contributors or members of our Discord, or any other individual was, is, or ever will be responsible for any damage done to your console, other property, yourself or others.
{: .notice--warning }

Before attempting to carry out any guide in this website or following any external links, we recommend reading the **entire** page _at least_ once, to get a general idea of what to do and how to do it.
This can also help prevent unnecessary purchases, so you know how and if you can carry out the mod before spending money on any tools or parts.
If something doesn't quite make sense, you can try visualising how it will work by looking at the Wii mini board in front of you, while not having any tools near you. If it still doesn't make sense and you need help, feel free to join our Discord server linked above. 
{: .notice--info }

To prevent from bricking your console, do NOT install **ANY** IOSes without being instructed by this guide or wii.guide's Wii mini-specific pages without having a WiFi module installed. You should also never follow any video tutorials that do not directly link to this website or wii.guide.
{: .notice--danger}

### You will need

- A standard Phillips #0 screwdriver
- A good quality soldering iron with a flat but fine tip. If you're looking for a good but cheap option, we recommend the miniware TS100/TS80 series or the Pine64 Pinecil (not affiliated with either, we just use them in the community and find them really cool and easy to use).
- Thin solder, optionally rosin core
- Flux in either pen, liquid, syringe or paste form, depending on your preference (optional but highly recommended for more advanced mods).
- Multimeter with resistance or continuity mode, useful for diagnosing 

We will not teach you how to use any of these tools, simply because this guide is not for beginners to soldering, but if you are really determined you can try a soldering practice kit and look up guides and tutorials online.

### Softmodding

Most of these mods require basic access to homebrew on the Wii mini, so you should first follow our sibling softmodding guide at [wii.guide](https://wii.guide) from Bluebomb all the way to d2xl cios. For any help with that, feel free to join the Wii mini hacking Discord, linked at the top of this page.

Follow the instructions for modding your console with Bluebomb, installing the Homebrew channel and Priiloader. Read all the Dos and Dont's of Wii modding, but do not proceed to installing cIOS if you haven't already, it's not needed at the moment and may actually complicate the process.

### Teardown

Once you have read, acquired and completed all of the above, you can start by taking apart your console.

[This excellent guide](https://www.ifixit.com/Guide/Nintendo+Wii+mini+Motherboard+Replacement/37774) on iFixit can help you with that. Follow it until the end and make sure to store your screws and little parts somewhere safe if you don't plan to immediately close your console back. 

Please be extra cautious when fiddling with the power button board, as the ribbon cable is rather delicate and can get damaged easily. Also make sure to store the disc drive module in an enclosed container if you plan to stow it for a long time, as dust and debris can damage the laser head or carriage.
{: .notice--info }

You should now have the Wii mini board outside its casing and ready to be worked on. Please note that for the console to boot in its current state, the bluetooth card and disc drive sub-board need to be attached. The disc drive mechanism itself is not needed, so you can *very* gently disconnect the 3 ribbon cables of the black disc drive assembly from the back of the disc drive driver board and unhook it. Again, store that in a safe and dust-free environment.

While the console will boot without a heatsink or fan, it is not designed to run passively so keep an eye on its temperature and do not leave it running for any more than absolutely necessary. You should also refrain from running any games or demanding software without active cooling.
{: .notice--warning }

The thermal pads and paste used to attach the CPU and GPU to the heatsink are not strictly reusable, but if you avoid leaving any marks or fingerprints on them while working on the board you _could_ reuse them. Since most mods are performed on the back side of the board, you can also keep the top metal shield attached to the motherboard to protect the thermal solution. If you want to replace them, remove them off the chips and the metal shield by scraping and cleaning with IPA or another 90%+ unscented alcohol solution and reapply pads of identical thickness to the originals.
{: .notice--info }

### The Saga Begins

Once you've read all of the above, you can proceed to [pick-a-pimp](pick-a-pimp)
{: .notice--info }