---
layout: add
type: action
title: Adding Standards
yaml: standard.yml
---

<div id="standards">
<p>Standards are metadata schemes used in a research data setting</p>
<h3>Standard Template</h3>
{% include implementation.html type='standard' %}
<h3>Instructions</h3>
<ol>
<li>
  Copy template: <button class="clip-button btn btn-primary" title="copy to
                         clipboard" type="button" 
                         data-clipboard-text="{% include {{page.yaml}} %}">
    Copy to Clipboard</button>
</li>
<li>Goto GitHub: <a href="{{ site.repourl }}/new/{{ site.repobranch }}/standards">
    Add a new file</a>
  <ol>
    <li>This will fork a copy of the site's repository and allow you to edit a
        page.</li>
  </ol>
</li>
<li>Paste in your boilerplate and edit away!</li>
<li>Commit and then submit a pull request</li>
</ol>
</div>
