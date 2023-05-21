---
title: Team
nav:
  order: 1
  tooltip: Who we are
---

# {% include icon.html icon="fa-solid fa-users" %}Team


{% include list.html data="members" component="portrait" filters="role: pi" style="large"  style="medium"   %}
{% include list.html data="members" component="portrait" filters="role: postdoc"   style="medium"  %}
{% include list.html data="members" component="portrait" filters="role: phd"  style="medium"  %}
{% include section.html background="images/background.jpg" dark=true %}

{% include section.html %}


# {% include icon.html icon="fa-solid fa-graduation-cap" %}Alumni

{% include list.html data="members" component="portrait" filters="role: alum" style="medium"  %}

{% include section.html background="images/background.jpg" dark=true %}

{% include section.html %}
# {% include icon.html icon="fa-solid fa-paw" %}Technical support

{% capture content %}
{% include list.html data="pets" component="portrait" filters="role: pet" style="small" %}
{% endcapture %}
{% include grid.html style="square" content=content   %}
