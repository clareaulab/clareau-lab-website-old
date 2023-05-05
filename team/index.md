---
title: Team
nav:
  order: 1
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team


{% include list.html data="members" component="portrait" filters="role: pi" %}
{% include list.html data="members" component="portrait" filters="role: ^(?!pi$)" %}

{% include section.html background="images/background.jpg" dark=true %}

{% include section.html %}

# {% include icon.html icon="fa-solid fa-paw" %}Technical support

{% capture content %}

{% include figure.html image="images/pets/boo.png" caption="Boo"  %}
{% include figure.html image="images/pets/nala.png" caption="Nala"  %}

{% endcapture %}

{% include grid.html style="square" content=content   %}
