---
title: Contact
nav:
  order: 6
  tooltip: Contact us
---
{% include section.html size="full"%}

{% include figure.html image="images/nyc-crappy.svg"  height="80" unit="%" %}

{% include section.html %}

# {% include icon.html icon="fa-regular fa-envelope" %}Contact


{% include section.html dark=false %}

{% capture col1 %}
Lareau Lab
417 East 68th Street
Zuckerman Research Center, 11th Floor
New York, NY 10065
{% endcapture %}

{% capture col2 %}
 
{% endcapture %}

{% capture col3 %}

{% endcapture %}

{% include cols.html col1=col1 col2=col2 col3=col3 %}


{% include section.html size = "full"%}

{% include figure.html name="Zuckerman" image="images/zuckerman.jpg" %}

{%
  include button.html
  type="email"
  text="Email Caleb"
  link="caleb.lareau@gmail.com"
%}
