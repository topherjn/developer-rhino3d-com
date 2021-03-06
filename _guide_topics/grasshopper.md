---
title: Grasshopper Guides
description: Guides to creating custom Grasshopper components and plugins.
platforms: ['Windows']
layout: guide-homepage
---

<!--the .snagit project for this image can be found next to the image -->
[<img src="{{ site.baseurl }}/images/grasshopper-guides-col1.png">]({{ site.baseurl }}/guides/grasshopper/what-is-a-grasshopper-component/)

### Overview

- [What is a Grasshopper Component?]({{ site.baseurl }}/guides/grasshopper/what-is-a-grasshopper-component/)

### Getting Started

- [Installing Tools]({{ site.baseurl }}/guides/grasshopper/installing-tools-windows/)
- [Your First Component]({{ site.baseurl }}/guides/grasshopper/your-first-component-windows/)

<!--column-->

<!--the .snagit project for this image can be found next to the image -->
[<img src="{{ site.baseurl }}/images/grasshopper-guides-col2.png">]({{ site.baseurl }}/guides/grasshopper/simple-component/)

### Fundamentals

<div class="trigger">
  {% assign guides = site.guide_topics | sort:"order" %}
  <ul>
  {% for guide in guides %}
    {% if guide.sdk contains 'Grasshopper' and guide.categories contains 'Fundamentals' %}
      {% if guide.title and guide.order %}
        <li><a class="page-link" href="{{ guide.url | prepend: site.baseurl }}" title="{{ guide.description }}">{{ guide.title }}</a></li>
      {% endif %}
    {% endif %}
  {% endfor %}
  </ul>
</div>

### Advanced

<div class="trigger">
  {% assign guides = site.guide_topics | sort:"order" %}
  <ul>
  {% for guide in guides %}
    {% if guide.sdk contains 'Grasshopper' and guide.categories contains 'Advanced' %}
      {% if guide.title and guide.order %}
        <li><a class="page-link" href="{{ guide.url | prepend: site.baseurl }}" title="{{ guide.description }}">{{ guide.title }}</a></li>
      {% endif %}
    {% endif %}
  {% endfor %}
  </ul>
</div>

<!--column-->

<!--the .snagit project for this image can be found next to the image -->
[<img src="{{ site.baseurl }}/images/grasshopper-guides-col3.png">]({{ site.baseurl }}/guides/grasshopper/grasshopper-data-types/)

### In Depth

<div class="trigger">
  {% assign guides = site.guide_topics | sort:"order" %}
  <ul>
  {% for guide in guides %}
    {% if guide.sdk contains 'Grasshopper' and guide.categories contains 'In Depth' %}
      {% if guide.title and guide.order %}
        <li><a class="page-link" href="{{ guide.url | prepend: site.baseurl }}" title="{{ guide.description }}">{{ guide.title }}</a></li>
      {% endif %}
    {% endif %}
  {% endfor %}
  </ul>
</div>
