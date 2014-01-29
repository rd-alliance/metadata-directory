---
title: Standards
layout: base
type: index

---
{% for subject in site.data.subjects %}
## {{ subject.label }}
<dl>
{% for page in site.pages %}
{% if page.subjects contains subject.value and page.type contains 'standard' %}
<dt>
  <a href="{{ page.website }}">{{ page.title }}</a>
  <a href="{{site.repourl}}/edit/{{ site.repobranch }}/standards/{{page.name}}.md"
     class="btn btn-default btn-xs" role="button">
    <span class="glyphicon glyphicon-edit"></span> Edit</a>
</dt>
<dd>{{ page.description }}</dd>
{% endif %}
{% endfor %}
</dl>
{% endfor %}
    
