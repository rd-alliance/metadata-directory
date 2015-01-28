---
title: Subject Areas
name: index
layout: links
type: index

---
{% for subject in site.data.subjects %}
<h2>{{ subject.label }}</h2>
<dl>
{% assign sortedPages = site.pages | sort:"name" %}
{% for page in sortedPages %}
{% if page.subjects contains subject.value and page.type contains 'standard' %}
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
{% endfor %}
    
