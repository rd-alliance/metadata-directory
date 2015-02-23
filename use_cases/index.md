---
title: Use Cases
name: index
layout: links
type: index

---
{% assign sortedPages = site.pages | sort:"name" %}
{% for area in sortedPages %}
{% if area.type == 'subject' %}
<h2>{{ area.title }}</h2>
<dl>
<h2>{{ subject.label }}</h2>
<dl>
{% for page in sortedPages %}
{% if page.subjects contains area.name and page.type contains 'use_case' %}
<dt>
  <a href="{{ page.website | escape }}">{{ page.title }}</a>
  <a href="{{site.repourl}}/edit/{{ site.repobranch }}/use_cases/{{page.name}}"
     class="btn btn-default btn-xs" role="button">
    <span class="glyphicon glyphicon-edit"></span> Edit</a>
</dt>
<dd>{{ page.description }}</dd>
{% endif %}
{% endfor %}
</dl>
{% endif %}
{% endfor %}
