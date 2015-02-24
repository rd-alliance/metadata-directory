---
title: Standards
slug: index
layout: links
type: index

---
{% assign subjectAreas = site.pages | where:'type','subject' | sort:"sort" %}
{% assign standards = site.pages | where:'type','standard' | sort:"name" %}
{% for area in subjectAreas %}
<h2>{{ area.title }}</h2>
<dl>
{% for standard in standards %}
{% if standard.subjects contains area.slug %}
<dt>
  <a href="{{ site.baseurl }}{{ standard.url }}">{{ standard.title }}</a>
  <a href="{{site.repourl}}/edit/{{ site.repobranch }}/standards/{{standard.name}}" class="btn btn-default btn-xs" role="button">
    <span class="glyphicon glyphicon-edit"></span> Edit</a>
</dt>
<dd>{{ standard.description }}</dd>
{% endif %}
{% endfor %}
</dl>
{% endfor %}