---
title: Use Cases
slug: index
layout: links
type: index

---
{% assign subjectAreas = site.pages | where:'type','subject' | sort:"sort" %}
{% assign usecases = site.pages | where:'type','use_case' | sort:"name" %}
{% for area in subjectAreas %}
<h2>{{ area.title }}</h2>
<dl>
{% for usecase in usecases %}
{% if usecase.subjects contains area.slug %}
<dt>
  <a href="{{ usecase.website | escape }}">{{ usecase.title }}</a>
  <a href="{{site.repourl}}/edit/{{ site.repobranch }}/use_cases/{{usecase.name}}" class="btn btn-default btn-xs" role="button">
    <span class="glyphicon glyphicon-edit"></span> Edit</a>
</dt>
<dd>{{ usecase.description }}</dd>
{% endif %}
{% endfor %}
</dl>
{% endfor %}
