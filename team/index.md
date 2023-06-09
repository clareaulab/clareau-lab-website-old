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


{% include section.html background="images/scistories.jpg" dark=true %}
{% include section.html %}


# {% include icon.html icon="fa-solid fa-graduation-cap" %}Alumni

{% include list.html data="members" component="portrait" filters="role: alum" style="medium"  %}

{% include section.html background="images/scistories.jpg" dark=true %}

{% include section.html %}
# {% include icon.html icon="fa-solid fa-paw" %}Technical support


{% include portrait.html name="Alpha" style="small" image="images/pets/alpha.png" %}
{% include portrait.html name="Boo" style="small" image="images/pets/boo.png" %}
{% include portrait.html name="Brooks" style="small" image="images/pets/brooks.png" %}
{% include portrait.html name="Nala" style="small" image="images/pets/nala.png" %}

{% capture content %}
{% include list.html data="pets" component="portrait" filters="role: pet" style="small" %}
{% endcapture %}
{% include grid.html style="square" content=content   %}
