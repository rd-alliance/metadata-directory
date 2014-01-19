---
title: Standards
layout: base
theme: standards
---
{% for discipline in site.data.disciplines %}
## {{ discipline | capitalize}}
{% for page in site.pages %}
{% if page.disciplines contains discipline %}
[{{ page.title }}]({{ page.url }})
{% endif %}
{% endfor %}
{% endfor %}

    
