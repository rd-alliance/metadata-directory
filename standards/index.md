---
title: Standards
layout: base
type: index

---
{% for subject in site.data.subjects %}
## {{ subject.label }}
{% for page in site.pages %}
{% if page.subjects contains subject.value and page.type contains 'standard'  %}
<!-- Liquid can't provide a relative URL -->
[{{ page.title }}]({{ site.baseurl }}{{ page.url }})
:  {{ page.description }}
{% endif %}
{% endfor %}
{% endfor %}

    
