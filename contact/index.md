---
title: Contact
nav:
  order: 6
  tooltip: Contact us
---

{% include section.html %}

# {% include icon.html icon="fa-solid fa-magnifying-glass" %}Contact


{% capture col1 %}
<b>Lareau Lab</b><br>
417 East 68th Street<br>
Zuckerman Research Center, 11th Floor<br>
New York, NY 10065
{% endcapture %}

{% capture col2 %}
 
{% endcapture %}

{% capture col3 %}
<br>
{%
  include button.html
  type="email"
  text="Email Caleb"
  link="caleb.lareau@gmail.com"
%}
<br>
{% endcapture %}

{% include cols.html col1=col1 col2=col2 col3=col3 %}


{% include section.html size = "wide"%}

{% include figure.html name="Zuckerman" image="images/zuckerman.jpg" %}
