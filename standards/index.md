---
title: Standards
name: index
layout: base
type: index

---
<dl>
{% assign sortedPages = site.pages | sort_by:name %}
{% for page in sortedPages %}
{% if page.type contains 'standard' %}
<dt>
  <a href="{{ site.baseurl }}{{ page.url }}">{{ page.title }}</a>
  <a href="{{site.repourl}}/edit/{{ site.repobranch }}/standards/{{page.name}}.md"
     class="btn btn-default btn-xs" role="button">
    <span class="glyphicon glyphicon-edit"></span> Edit</a>
</dt>
<dd>{{ page.description }}</dd>
{% endif %}
{% endfor %}
</dl>
