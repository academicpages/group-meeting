---
layout: layout
title: "About"
---

<!-- You can edit this whole page, remove it, or use it as basis for any non-post pages you have. -->
<section class="content">

# {{ site.name }}

<ul class="listing">
<li>
<span>Fall 2018</span><a href="{{ site.url }}/upcoming.html">Upcoming Topics</a>
</li>
  {% assign upcoming = (site.posts | where: "category" , "upcoming") %}
  {% for post in upcoming reversed %}
    {% if forloop.first %}
    <li style="text-indent: 2em;">
	<span>{{ post.date | date: "%B %e, %Y" }}</span> Next topic: <a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a>
	</li>
    {% endif %}
  {% endfor %}
<li>
<span>2015-2016</span><a href="{{ site.url }}/previous.html">Previous Topics</a>
</li>
</ul>


## What:

This is a description of your group.

## Where:

This is where your group's meetings are held.

## When:

This is when your group meets.

## How:

### Participation

This is how you participate in your group.

### Communications

Links to various lists and chat services.

</section>
