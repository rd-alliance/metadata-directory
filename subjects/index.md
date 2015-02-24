---
title: Subject Areas
slug: index
layout: links
type: index
---
{% assign sortedPages = site.pages | sort:"name" %}
{% for area in sortedPages %}
{% if area.type == 'subject' %}
<h2>
  <a href="{{ site.baseurl }}{{ area.url }}">{{ area.title }}</a>
  <a href="{{ site.repourl }}/edit/{{ site.repobranch }}/subjects/{{ area.name }}" class="btn btn-default btn-xs" role="button">
    <span class="glyphicon glyphicon-edit"></span> Edit</a>
</h2>
<ul>
{% for page in sortedPages %}
{% if page.subjects contains area.slug and page.type contains 'discipline' %}
<li>
  <a href="{{ site.baseurl }}{{ page.url }}">{{ page.title }}</a>
  <a href="{{ site.repourl }}/edit/{{ site.repobranch }}/subjects/{{ page.name }}" class="btn btn-default btn-xs" role="button">
    <span class="glyphicon glyphicon-edit"></span> Edit</a>
</li>
{% endif %}
{% endfor %}
</ul>
{% endif %}
{% endfor %}
