---
title: "Site Navigation" #
layout: single
sitemap: false
---
<!--![WiiTutorials](/images/WiiTutorials.jpg) TODO: Add Wiini image-->

{% capture notice-1 %}
**Featured**

+ [Pick-A-Pimp](pick-a-pimp)
{% endcapture %}
<div class="notice--info">{{ notice-1 | markdownify }}</div>

{% capture notice-2 %}

**Hardware Mods**
+ [Reset Switch](reset)
+ [SD Card Slot](sdcard)

**Custom Add-in Boards**
+ [TBA: WiiMini-SDRST by WebHDX](sdrst)
+ [miniRGBii Component Filter Board by Job and Devnol](miniRGBii)

**Software Mods**
+ [Original System Menu install (no WiFi card)](sminstall-nowifi)
+ [Mii Channel restore removed functionality](mii-upgrade)

**Site**
+ [Home](/)
+ [Get Started](get-started)
+ [FAQ](faq)
+ [Donations](donations)
{% endcapture %}
<div class="notice--primary">{{ notice-2 | markdownify }}</div>
