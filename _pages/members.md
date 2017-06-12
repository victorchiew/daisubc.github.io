---
layout: page
title: Members
permalink: /members/
description: Current students and alumni.
---
<link rel="stylesheet" href="{{ '/assets/css/members.css' | prepend: site.baseurl | prepend: site.url }}">

<div class="toolbar">
  <button class="btn fil-cat" href="" data-rel="All">All</button>
  <button class="btn fil-cat" data-rel="PhD">PhD</button>
  <button class="btn fil-cat" data-rel="MASc">MASc</button>
  <button class="btn fil-cat" data-rel="BAsc">BAsc</button>
  <button class="btn fil-cat" data-rel="Current">Current</button>
  <button class="btn fil-cat" data-rel="Alumni">Alumni</button>
</div> 

<hr>
<div id="members">
{% for member in site.members %}
    <a class="tile All {{ member.program }} {{ member.status }}" href="{{ member.url | prepend: site.baseurl | prepend: site.url }}"> 
        <figure>
            <img src="{{ member.img | prepend: site.baseurl | prepend: site.url }}">
            <figcaption>    
            <b> {{ member.title }} </b> | {{ member.program }}
            </figcaption>
        </figure>
    </a>
{% endfor %}
</div>
