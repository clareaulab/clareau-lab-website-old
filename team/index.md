---
title: Team
nav:
  order: 1
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team


{% include list.html data="members" component="portrait" filters="role: pi" %}
{% include list.html data="members" component="portrait" filters="role: postdoc" %}
{% include list.html data="members" component="portrait" filters="role: phd" %}

{% include section.html background="images/background.jpg" dark=true %}

{% include list.html data="members" component="portrait" filters="role: alum" %}

{% include section.html %}

# {% include icon.html icon="fa-solid fa-paw" %}Technical support

{% capture content %}

{% include list.html data="members" component="portrait" filters="role: pet" %}

{% endcapture %}

{% include grid.html style="square" content=content   %}
