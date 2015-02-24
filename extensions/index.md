---
title: Extensions
slug: index
layout: links
type: index

---
{% assign subjectAreas = site.pages | where:'type','subject' | sort:"sort" %}
{% assign extensions = site.pages | where:'type','extension' | sort:"name" %}
{% for area in subjectAreas %}
<h2>{{ area.title }}</h2>
<dl>
{% for extension in extensions %}
{% if extension.subjects contains area.slug %}
<dt>
  <a href="{{ extension.website | escape }}">{{ extension.title }}</a>
  <a href="{{site.repourl}}/edit/{{ site.repobranch }}/extensions/{{extension.name}}" class="btn btn-default btn-xs" role="button">
    <span class="glyphicon glyphicon-edit"></span> Edit</a>
</dt>
<dd>{{ extension.description }}</dd>
{% endif %}
{% endfor %}
</dl>
{% endfor %}
