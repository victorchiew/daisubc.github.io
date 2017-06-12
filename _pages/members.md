---
layout: page
title: Group Members
permalink: /members/
description: Current students and alumni.
---

<div class="toolbar">
  <button class="btn fil-cat" href="" data-rel="All">All</button>
  <button class="btn fil-cat" data-rel="PhD">PhD</button>
  <button class="btn fil-cat" data-rel="MASc">MASc</button>
  <button class="btn fil-cat" data-rel="BAsc">BAsc</button>
</div> 

<hr>
<div id="members">
{% for member in site.members %}
<ul>
<li class= "All {{ member.program }}" >
    <a href="{{ member.url | prepend: site.baseurl | prepend: site.url }}"> 
    <span>
        <b> {{ member.title }} </b>
        <br>
        {{ member.program }}
    </span>
    </a>
</li>

</ul>
{% endfor %}
</div>
