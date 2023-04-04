---
layout: add
slug: add
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
  <li>
    <p>Copy template:
      <button class="clip-button btn btn-primary" title="copy to clipboard" type="button"
        data-clipboard-text="{% include {{page.yaml}} %}">Copy to Clipboard</button></p>
  </li>
  <li>
    <p>Go to GitHub:
      <a href="{{ site.repourl }}/new/{{ site.repobranch }}/tools">Add a new file</a></p>
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
