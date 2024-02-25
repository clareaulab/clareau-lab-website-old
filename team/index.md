---
title: Team
nav:
  order: 1
  tooltip: Who we are
carousels:
  - images: 
    - image: /images/group/holidayparty2023.jpg
    - image: /images/group/playthatgoeswrong.png
    - image: /images/group/pizza1.jpg

---



# {% include icon.html icon="fa-solid fa-users" %}Team


{% include list.html data="members" component="portrait" filters="role: pi" style="medium"   %}
{% include list.html data="members" component="portrait" filters="role: admin"   style="medium"  %}
{% include list.html data="members" component="portrait" filters="role: srtech"   style="medium"  %}
{% include list.html data="members" component="portrait" filters="role: postdoc"   style="medium"  %}
{% include list.html data="members" component="portrait" filters="role: mdstu"  style="medium"  %}
{% include list.html data="members" component="portrait" filters="role: phd"  style="medium"  %}


{% include section.html background="images/scistories-clear-cut.png" dark=false %}
{% include section.html %}

{% include carousel.html height="40" unit="%" duration="10" number="1" %}

{% include section.html background="images/scistories-clear.png" dark=false %}



# {% include icon.html icon="fa-solid fa-graduation-cap" %}Alumni

{% include list.html data="members" component="portrait" filters="role: alum" style="medium"  %}

{% include section.html background="images/scistories-clear-cut.png" dark=false %}

{% include section.html %}
# {% include icon.html icon="fa-solid fa-paw" %}Technical support


{% include portrait.html name="Alpha" style="small" image="images/pets/alpha.png" %}
{% include portrait.html name="Boo" style="small" image="images/pets/boo.png" %}
{% include portrait.html name="Brooks" style="small" image="images/pets/brooks.png" %}
{% include portrait.html name="Kinzo" style="small" image="images/pets/kinzo.png" %}
{% include portrait.html name="Luna" style="small" image="images/pets/luna.png" %}
{% include portrait.html name="Nala" style="small" image="images/pets/nala.png" %}
{% include portrait.html name="Ono" style="small" image="images/pets/ono.png" %}
{% include portrait.html name="Sabrina" style="small" image="images/pets/sabrina.png" %}
{% include portrait.html name="Zuka" style="small" image="images/pets/zuka.png" %}

{% capture content %}
{% include list.html data="pets" component="portrait" filters="role: pet" style="small" %}
{% endcapture %}
{% include grid.html style="square" content=content   %}
