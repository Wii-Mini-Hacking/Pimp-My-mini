---
layout: splash
title: "Pimp My mini"
header:
  overlay_color: "#5e616c"
  overlay_image: /images/home-page-feature.jpg
  overlay_filter: 0.5
  caption:
excerpt: "The complete guide to hardware modding your Nintendo Wii mini"
---

<!--The guide is also available in other languages! To change the language, please press the icon at top right and change your language.
{: .notice--info}-->

This guide is a work-in-progress. Please do not use this guide if you read this message. Instead, you can visit our Discord server linked above for help and manual support.
{: .notice--warning}

## So what is "hardware modding"?

Hardware modding, or hardmodding for short, is the act of modifying an off-the-shelf commercial device, such as a console, to allow it to achieve things that were previously not possible simply by the use of software (either retail or [Homebrew](https://en.wikipedia.org/wiki/Homebrew_(video_games))).

## But what's the deal with the Wii mini?

The Wii mini (model RVL-201, hereafter referred to as "Wiini" for short), was a severely cut-down version of the original Wii, designed by Nintendo in a very cost-effective manner in order to get rid of old chip stock and get every last penny possible from the popularity of the Wii, before it was discontinued and replaced by its flawed successor, the Wii U. Specifically, the Wii mini lacks the following features compared to the original Wii (RVL-001):

- **Reset Button**: Not particularly useful for normal use as the Home pause menu had a reset option, however necessary for some homebrew tools.
- **SD Card Slot**: Used by some games such as the Super Smash Bros. Brawl and a lot of homebrew, especially older ones.
- **WiFi Connectivity**: Nintendo WiFi Connection and WiiConnect24 was discontinued shortly after the Wii mini's release, so including networking support was fairly redundant. However, [Wiimmfi](https://wiimmfi.de) and [RiiConnect24](https://rc24.xyz) can now restore most missing network features, however they do require some hardware modding for use on the wiini.
- **Ethernet Connection**: Similarly to WiFi, Nintendo also removed support for the Wii LAN Adapter for wired networking. Basic functionality for it can be restored using just software, but it isn't particularly useful since Wiimmfi and RC24 still require hardware modding.  
- **Component Video**: The Wii mini AV out port, while it's identical to the one on the regular Wii, can only output Composite Video (Yellow coaxial cable) in either 480i or 576i (interlaced). It does not support the crisper 480p output that Component (YPbPr) Provides
- **Second USB Port**: The Wii mini only has 1 USB port instead of 2, again probably as an extreme cost-cutting measure, since the games that needed more than 1 port (and didn't require internet) were next to none.
- **GameCube Backwards Compatibility**: Similarly to the Wii Family Edition (RVL-101), the Wiini does not have any hardware support for playing GameCube discs, using GameCube controllers and Memory Cards and anything else that utilises those ports.
- **Software Features**: Apps that require any of the above features are removed, and others are stripped down. For example, the Photo, Forecast, Everybody Votes and News channels are all removed and the Mii Channel has the Mii Parade and sharing functions disabled.

Even then, the Wii mini still sold an acceptable amount of units (though specific numbers are unknown), especially to young children or elderly people, due to its really low cost (MSRP of around 99 USD) and large back-catalog of games. If you're just looking for a Wii to play games on, we wouldn't recommend getting a Wiini, since a used non-mini Wii costs less and provides more features. However, if you happen to already own one or are simply interested in its modding potential, this guide is just right for you.
## Ready?

Well... we're not, so you're gonna have to wait a little. In the meantime, you can join [our Discord server](https://discord.gg/6ryxnkS) for discussion, support or to help us complete this website!
{: .notice--info}

Continue to [Getting Started](get-started)
{: .notice--info}

## Credits
This modding scene, and by extension this website wouldn't be possible without the help of some amazing people:

- ProfessionalThonker/CaveStoryKing64: Having the perseverance and sheer testicle girth to organise and maintain such a futile and pointless scene
- Fullmetal5: Bluebomb exploit and misc software black magic
- DeadlyFoez: Initial hardware exploration, experimentation and poking around. Credit for all Wii mini board images goes to him, unless otherwise noted.
- DestroyedEdge: Being edgy
- Aurelio: for his RVLoader installer software adapted for the Wiini sd patcher
- WiiMaster: for helping me test the awful changes I made to above software
- Job, Webhdx et. al: Making custom boards and extending what's possible with the console
- Nintendo R&D: for giving us something cool to play with
- Terry A. Davis: Inspiration and motivation

_Our thoughts and prayers go out to the Wii mini victims of the WiFi IOS plague and all those who sacrificed their lives in the hands of DeadlyFoez in the name of science._