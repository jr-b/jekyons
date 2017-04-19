---
layout: page
title:  "Blogue"
permalink: /blogue.html
---

<div class="pa2">

  {% for post in site.posts %}

  <h3 class="mb1 pb1"><a class="link navy ba pa1 bg-animate hover-bg-near-white" href="{{ post.url }}">{{ post.title }}</a></h3>

  <p class="mt1 pt1 mb3"><strong>{{ post.date | date: "%B %d, %Y" }}</strong>. <span class="i o-70">{{ post.categories | join: ', ' }}</span>

  <a href="{{ post.url }}"></a>

  </p>

  {% endfor %}

</div>
