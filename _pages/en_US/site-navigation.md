---
title: "Site Navigation" #
layout: single
sitemap: false
---
![WiiTutorials](/images/WiiTutorials.jpg)

{% capture notice-1 %}
**Featured**

+ [Pick-A-Pimp](pick-a-pimp)
{% endcapture %}
<div class="notice--info">{{ notice-1 | markdownify }}</div>

{% capture notice-2 %}

**Generic Mods**
+ [Reset Switch](reset)
+ [SD Card Slot](sdcard)

**Custom Add-in Boards**
+ [WiiMini-SDRST by WebHDX](sdrst)
+ [miniRGBii Component Filter Board by Job and Devnol](miniRGBii)

**Site**
+ [Home](/)
+ [Get Started](get-started)
+ [FAQ](faq)
+ [Donations](donations)
{% endcapture %}
<div class="notice--primary">{{ notice-2 | markdownify }}</div>
