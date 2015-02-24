---
title: Extensions
slug: index
layout: links
type: index

---
{% assign sortedPages = site.pages | sort:"name" %}
{% for area in sortedPages %}
{% if area.type == 'subject' %}
<h2>{{ area.title }}</h2>
<dl>
{% for page in sortedPages %}
{% if page.subjects contains area.slug and page.type contains 'extension' %}
<dt>
  <a href="{{ page.website | escape }}">{{ page.title }}</a>
  <a href="{{site.repourl}}/edit/{{ site.repobranch }}/extensions/{{page.name}}"
     class="btn btn-default btn-xs" role="button">
    <span class="glyphicon glyphicon-edit"></span> Edit</a>
</dt>
<dd>{{ page.description }}</dd>
{% endif %}
{% endfor %}
</dl>
{% endif %}
{% endfor %}
