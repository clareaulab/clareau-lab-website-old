---
title: Team
nav:
  order: 1
  tooltip: Who we are
---



# {% include icon.html icon="fa-solid fa-users" %}Team


{% include list.html data="members" component="portrait" filters="role: pi" style="medium"   %}
{% include list.html data="members" component="portrait" filters="role: admin"   style="medium"  %}
{% include list.html data="members" component="portrait" filters="role: srtech"   style="medium"  %}
{% include list.html data="members" component="portrait" filters="role: jrtech"   style="medium"  %}
{% include list.html data="members" component="portrait" filters="role: postdoc"   style="medium"  %}
{% include list.html data="members" component="portrait" filters="role: clinicalfellow"  style="medium"  %}
{% include list.html data="members" component="portrait" filters="role: mdstu"  style="medium"  %}
{% include list.html data="members" component="portrait" filters="role: mdph"  style="medium"  %}
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
{% include portrait.html name="Charlie" style="small" image="images/pets/charlie.png" %}
{% include portrait.html name="Choumao" style="small" image="images/pets/choumao.png" %}
{% include portrait.html name="Fiete" style="small" image="images/pets/fiete.png" %}
{% include portrait.html name="Ginny" style="small" image="images/pets/ginny.png" %}
{% include portrait.html name="Kinzo" style="small" image="images/pets/kinzo.png" %}
{% include portrait.html name="Luna" style="small" image="images/pets/luna.png" %}
{% include portrait.html name="Molle" style="small" image="images/pets/molle.png" %}
{% include portrait.html name="Nala" style="small" image="images/pets/nala.png" %}
{% include portrait.html name="Nacho" style="small" image="images/pets/nacho.png" %}
{% include portrait.html name="Playoff P" style="small" image="images/people/paul-dog.png" %}
{% include portrait.html name="Pixel" style="small" image="images/pets/pixel.png" %}
{% include portrait.html name="Rosie" style="small" image="images/pets/rosie.png" %}

{% capture content %}
{% include list.html data="pets" component="portrait" filters="role: pet" style="small" %}
{% endcapture %}
{% include grid.html style="square" content=content   %}
