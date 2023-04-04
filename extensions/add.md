---
layout: add
slug: add
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
  <li>
    <p>Copy template:
      <button class="clip-button btn btn-primary" title="copy to clipboard" type="button"
        data-clipboard-text="{% include {{page.yaml}} %}">Copy to Clipboard</button></p>
  </li>
  <li>
    <p>Go to GitHub:
      <a href="{{ site.repourl }}/new/{{ site.repobranch }}/extensions">Add a new file</a></p>
    <p>This will fork a copy of the site's repository and allow you to edit a page.</p>
  </li>
  <li>
    <p>Paste in your boilerplate and edit away!</p>
  </li>
  <li>
    <p>Commit and then submit a pull request</p>
  </li>
</ol>
</div>
