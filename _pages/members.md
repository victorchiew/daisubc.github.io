---
layout: page
title: Group Members
permalink: /members/
description: Current students and alumni.
---

<h2>PhD</h2>
{% for member in site.members %}
<div class="member">
<ul>
{% if member.program == 'PhD' %}
<li>
    <a href="{{ member.url | prepend: site.baseurl | prepend: site.url }}"> 
    <span>
        <p>{{ member.title }}</p>
    </span>
    </a>
</li>
{% endif %}
</ul>
</div>

{% endfor %}

<h2>MASc</h2>
{% for member in site.members %}
<div class="member">
<ul>
{% if member.program == 'MASc' %}
<li>
    <a href="{{ member.url | prepend: site.baseurl | prepend: site.url }}"> 
    <span>
        <p>{{ member.title }}</p>
    </span>
    </a>
</li>
{% endif %}
</ul>
</div>

{% endfor %}

<h2>BASc</h2>
{% for member in site.members %}
<div class="member">
<ul>
{% if member.program == 'BASc' %}
<li>
    <a href="{{ member.url | prepend: site.baseurl | prepend: site.url }}"> 
    <span>
        <p>{{ member.title }}</p>
    </span>
    </a>
</li>
{% endif %}
</ul>
</div>

{% endfor %}