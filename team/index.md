---
title: Team
nav:
  order: 1
  tooltip: Who we are
---

{% capture hiring %} **The lab is recruiting at all levels.** [Email Caleb](mailto:lareauc@mskcc.org) to discuss a possible position. {% endcapture %}
{% include alert.html type="info" content=hiring %}


# {% include icon.html icon="fa-solid fa-users" %}Team


{% include list.html data="members" component="portrait" filters="role: pi" style="medium"   %}
{% include list.html data="members" component="portrait" filters="role: admin"   style="medium"  %}
{% include list.html data="members" component="portrait" filters="role: srtech"   style="medium"  %}
{% include list.html data="members" component="portrait" filters="role: postdoc"   style="medium"  %}
{% include list.html data="members" component="portrait" filters="role: phd"  style="medium"  %}


{% include section.html background="images/scistories-clear-cut.png" dark=false %}
{% include section.html %}


# {% include icon.html icon="fa-solid fa-graduation-cap" %}Alumni

{% include list.html data="members" component="portrait" filters="role: alum" style="medium"  %}

{% include section.html background="images/scistories-clear-cut.png" dark=false %}

{% include section.html %}
# {% include icon.html icon="fa-solid fa-paw" %}Technical support


{% include portrait.html name="Alpha" style="small" image="images/pets/alpha.png" %}
{% include portrait.html name="Boo" style="small" image="images/pets/boo.png" %}
{% include portrait.html name="Brooks" style="small" image="images/pets/brooks.png" %}
{% include portrait.html name="Kinzo" style="small" image="images/pets/kinzo.png" %}
{% include portrait.html name="Nala" style="small" image="images/pets/nala.png" %}
{% include portrait.html name="Ono" style="small" image="images/pets/ono.png" %}
{% include portrait.html name="Sabrina" style="small" image="images/pets/sabrina.png" %}
{% include portrait.html name="Zuka" style="small" image="images/pets/zuka.png" %}

{% capture content %}
{% include list.html data="pets" component="portrait" filters="role: pet" style="small" %}
{% endcapture %}
{% include grid.html style="square" content=content   %}
