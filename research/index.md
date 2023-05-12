---
title: Research
nav:
  order: 2
  tooltip: 
---

# {% include icon.html icon="fa-solid fa-wrench" %}Research

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

{% capture content %}**Now recruiting** We are hiring at all levels of the lab.{% endcapture %}
{% include alert.html type="info" content=content %}

{% capture content %}
{% include figure.html image="images/gifs/hydrop.gif" caption="Caption" height="200px" %}
{% endcapture %}
{% include float.html content=content %}
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
{% include float.html clear=true %}



{% capture content %}
{% include figure.html image="images/gifs/mitochondria.gif" caption="Caption" height="200px" %}
{% endcapture %}
{% include float.html content=content %}
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
{% include float.html clear=true %}



{% capture content %}
{% include figure.html image="images/gifs/DNK.gif" caption="Caption"  height="200px" %}
{% endcapture %}
{% include float.html content=content %}
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
{% include float.html clear=true %}


{% include tags.html tags="publication, resource, website" %}

{% include search-info.html %}

{% include section.html %}

## Featured

{% include list.html component="card" data="projects" filters="group: featured" %}

{% include section.html %}

## More

{% include list.html component="card" data="projects" filters="group: " style="small" %}
