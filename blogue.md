---
layout: page
title:  "Blogue"
permalink: /blogue.html
---

<div class="pa2">

  {% for post in site.posts %}

  <h3><a class="link navy ba pa1 bg-animate hover-bg-near-white" href="{{ post.url }}">{{ post.title }}</a></h3>

      <p><strong>{{ post.date | date: "%B %d, %Y" }}</strong>. <span class="i o-70">{{ post.categories | join: ', ' }}</span>

      <a href="{{ post.url }}"></a></p>

  {% endfor %}

</div>
