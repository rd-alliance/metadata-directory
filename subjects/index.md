---
title: Subject Areas
slug: index
layout: links
type: index
---
{% assign subjectAreas = site.pages | where:'type','subject' | sort:'sort' %}
{% assign disciplines = site.pages | where:'type','discipline' | sort:'name' %}
{% for area in subjectAreas %}
<h2>
  <a href="{{ site.baseurl }}{{ area.url }}">{{ area.title }}</a>
  <a href="{{ site.repourl }}/edit/{{ site.repobranch }}/subjects/{{ area.name }}" class="btn btn-default btn-xs" role="button">
    <span class="glyphicon glyphicon-edit"></span> Edit</a>
</h2>
<ul>
{% for discipline in disciplines %}
{% if discipline.subjects contains area.slug %}
<li>
  <a href="{{ site.baseurl }}{{ discipline.url }}">{{ discipline.title }}</a>
  <a href="{{ site.repourl }}/edit/{{ site.repobranch }}/subjects/{{ discipline.name }}" class="btn btn-default btn-xs" role="button">
    <span class="glyphicon glyphicon-edit"></span> Edit</a>
</li>
{% endif %}
{% endfor %}
</ul>
{% endfor %}
