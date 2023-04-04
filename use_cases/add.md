---
layout: add
slug: add
type: action
title: Adding Use Cases
yaml: use_case.yml
---
<div id="use_cases">
<p>Use cases are specific organizations or projects which use the standard to
  in a research data system or setting</p>
<h3> Use Case Template</h3>
{% include implementation.html type='use_case' %}
<h3>Instructions</h3>
<ol>
  <li>
    <p>Copy template:
      <button class="clip-button btn btn-primary" title="copy to clipboard" type="button"
        data-clipboard-text="{% include {{page.yaml}} %}">Copy to Clipboard</button></p>
  </li>
  <li>
    <p>Go to GitHub:
      <a href="{{ site.repourl }}/new/{{ site.repobranch }}/use_cases">Add a new file</a></p>
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
