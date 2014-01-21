---
title: Tools
layout: base
type: index

---
{% for subject in site.data.subjects %}
<!-- Can't capitalize -->
## {{ subject | capitalize }}
{% for page in site.pages %}
{% if page.subjects contains subject and page.type contains 'tool'  %}
<!-- Liquid can't provide a relative URL -->
[{{ page.title }}]({{ site.baseurl }}{{ page.url }})
:  {{ page.description }}
{% endif %}
{% endfor %}
{% endfor %}

    
