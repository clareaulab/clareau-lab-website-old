---
title: Join
nav:
  order: 5
  tooltip: Email, address, and location
---

# {% include icon.html icon="fa-regular fa-envelope" %}Join us!


{% capture content %}**Now recruiting**  The lab is recruiting at all levels.{% endcapture %}
{% include alert.html type="info" content=content %}

We are particularly interested in individuals with wet-bench 
backgrounds that seek mentored training in computational biology,
data science, genomics, and/or biotechnology. 

Prospective research technicians and postdoctoral associates should [contact Caleb directly](mailto:caleb.lareau@gmail.com).

Graduate students should come from one of these programs:
- Program A
- Program B
- Program C



{% include section.html %}

{% capture col1 %}

{%
  include figure.html
  image="images/immune.jpg"
  caption="Lorem ipsum"
%}

{% endcapture %}

{% capture col2 %}

{%
  include figure.html
  image="images/nyc.jpg"
  caption="Lorem ipsum"
%}

{% endcapture %}

{% include cols.html col1=col1 col2=col2 col3=col2 %}

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
