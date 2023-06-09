---
title: Home
carousels:
  - images: 
    - image: /images/circles.jpg
    - image: /images/nyc.jpg
---

# Lareau Lab @ Memorial Sloan Kettering

Established in 2023, our lab is part of the Computational and Systems Biology program at Sloan Kettering Institute. 
The lab is located on the 11th Floor of Zuckerman Research Center


{% include section.html size="full" %}

[![See our research,80%](/images/circles.jpg)](https://clareaulab.com/research/)
[![View our research,60%](/images/circles.jpg)](research)



{% include section.html %}


# Computational and Translational Immunology

{% include carousel.html height="30" unit="%" duration="10" number="1" %}


{% include section.html %}

{% capture immuno %}

{%
  include figure.html
  image="images/immune.jpg"
  caption="Our group focuses on questions involving the immune system and immunotherapies."
%}

{% endcapture %}

{% capture nycr %}

{%
  include figure.html
  image="images/nyc.jpg"
  caption="The lab is located in Zuckerman Research Center at Sloan Kettering in New York City."
%}

{% endcapture %}

{% capture csb %}

{%
  include figure.html
  image="images/cs.jpg"
  caption="We specialize in computational methods for massive-scale genomics data."
%}

{% endcapture %}

{% include cols.html col1=immuno col2=csb col3=nycr %}


