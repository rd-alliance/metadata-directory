---
layout: add
name: add
type: action
title: Adding Tools
yaml: tool.yml
---
<div id="tools">
<p>Tools are usually software applications designed and built to create,
  update, and maintain research data using a particular metadata standard.</p>
<h3>Tool Template</h3>
{% include implementation.html type='tool' %}

<h3>Instructions</h3>
<ol>
<li>Copy template: <button class="clip-button btn btn-primary" title="copy to
                         clipboard" type="button" 
                         data-clipboard-text="{% include {{page.yaml}} %}">
    Copy to Clipboard</button></li>
<li>Goto GitHub: <a href="{{ site.repourl }}/new/{{ site.repobranch }}/tools">
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
