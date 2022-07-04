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

**Site**
+ [Home](/)
+ [Get Started](get-started)
+ [FAQ](faq)
+ [Donations](donations)
{% endcapture %}
<div class="notice--primary">{{ notice-2 | markdownify }}</div>
