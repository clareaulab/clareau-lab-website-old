---
title: Join!
nav:
  order: 5
  tooltip: Email, address, and location
---

# {% include icon.html icon="fa-regular fa-envelope" %}Join us!

The lab is recruiting at all levels. We are particularly interested in recruiting individuals with wet-bench 
backgrounds that seek training in computational biology, data science, genomics, and/or biotechnology. 

Prospective research technicians and postdoctoral associates should [contact Caleb directly](mailto:caleb.lareau@gmail.com).

Graduate students should come from one of these programs.

{%
  include button.html
  type="email"
  text="caleb.lareau@gmail.com"
  link="caleb.lareau@gmail.com"
%}
{%
  include button.html
  type="phone"
  text="(580) 747 7796"
  link="+1-580-747-7796"
%}
{%
  include button.html
  type="address"
  tooltip="Our location on Google Maps for easy navigation"
  link="https://www.google.com/maps"
%}


{%
  include figure.html
  image="images/background-white.jpg"
  caption=""
%}

{% include section.html %}

{% capture col1 %}

{%
  include figure.html
  image="images/background-white.jpg"
  caption="Lorem ipsum"
%}

{% endcapture %}

{% capture col2 %}

{%
  include figure.html
  image="images/background-white.jpg"
  caption="Lorem ipsum"
%}

{% endcapture %}

{% include cols.html col1=col1 col2=col2 %}

{% include section.html dark=true %}

{% capture col1 %}
Lorem ipsum dolor sit amet  
consectetur adipiscing elit  
sed do eiusmod tempor
{% endcapture %}

{% capture col2 %}
Lorem ipsum dolor sit amet  
consectetur adipiscing elit  
sed do eiusmod tempor
{% endcapture %}

{% capture col3 %}
Lorem ipsum dolor sit amet  
consectetur adipiscing elit  
sed do eiusmod tempor
{% endcapture %}

{% include cols.html col1=col1 col2=col2 col3=col3 %}
