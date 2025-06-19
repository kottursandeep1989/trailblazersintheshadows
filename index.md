---
layout: default
title: Home
---

<h1 style="text-align:center; font-size: 2.5em;">🌍 Trailblazers in the Shadows</h1>
<p style="text-align:center; font-size: 1.2em;">
Celebrating 20 extraordinary women whose names deserve the spotlight. From Arctic survival to space missions, their impact spans every continent.
</p>

<div style="display:grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 1rem;">
{% for post in site.posts %}
  <div style="border: 1px solid #ccc; padding: 10px; border-radius: 8px;">
    <img src="{{ post.image }}" alt="{{ post.title }}" style="width:100%; height:180px; object-fit:cover; border-radius: 6px;" />
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
  </div>
{% endfor %}
</div>
