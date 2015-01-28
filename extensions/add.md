---
layout: add
name: add
type: action
title: Adding Extensions
yaml: extension.yml
---
<div id="extensions">
<p>Extensions are additions to an existing metadata standard that enables
additional functionality or meet other functional requirements.</p>
<h3>Extension Template</h3>
{% include implementation.html type='extension' %}

<h3>Instructions</h3>
<ol>
<li>Copy template: <button class="clip-button btn btn-primary"
                         title="copy to clipboard"
                         type="button"
                         data-clipboard-text="{% include {{page.yaml}} %}">
    Copy to Clipboard</button></li>
<li>Goto GitHub: <a href="{{ site.repourl }}/new/{{ site.repobranch }}/extensions">
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
