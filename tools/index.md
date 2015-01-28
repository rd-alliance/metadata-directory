---
title: Tools
name: index
layout: links
type: index

---
{% for subject in site.data.subjects %}
<h2>{{ subject.label }}</h2>
<dl>
{% for page in site.pages %}
{% if page.subjects contains subject.value and page.type == 'tool' %}
<dt>
  <a href="{{ page.website | escape }}">{{ page.title }}</a>
  <a href="{{site.repourl}}/edit/{{ site.repobranch }}/tools/{{page.name}}.md"
     class="btn btn-default btn-xs" role="button">
    <span class="glyphicon glyphicon-edit"></span> Edit</a>
</dt>
<dd>{{ page.description }}</dd>
{% endif %}
{% endfor %}
</dl>
{% endfor %}

    
