---
title: Tools
slug: index
layout: links
type: index

---
{% assign subjectAreas = site.pages | where:'type','subject' | sort:"sort" %}
{% assign tools = site.pages | where:'type','tool' | sort:"name" %}
{% for area in subjectAreas %}
<h2>{{ area.title }}</h2>
<dl>
{% for tool in tools %}
{% if tool.subjects contains area.slug %}
<dt>
  <a href="{{ tool.website | escape }}">{{ tool.title }}</a>
  <a href="{{site.repourl}}/edit/{{ site.repobranch }}/tools/{{tool.name}}" class="btn btn-default btn-xs" role="button">
    <span class="glyphicon glyphicon-edit"></span> Edit</a>
</dt>
<dd>{{ tool.description }}</dd>
{% endif %}
{% endfor %}
</dl>
{% endfor %}
