---
title: Metadata Directory
name: index
type: home
layout: base

---

[Prototype metadata directory]({{ site.baseurl }}/) for the Research Data Alliance.

* [Visit the standards]({{ site.baseurl }}/standards/)
* [Visit the extensions]({{ site.baseurl }}/extensions/)
* [Visit the tools]({{ site.baseurl }}/tools/)
* [Visit the use cases]({{ site.baseurl }}/use_cases/)

## Instructions

### [Adding a Standard]({{ site.baseurl }}/standards/add.html)

Adding a new standard is as simple as forking the repository creating a new
standards file marked up with a simple YAML schema. Commiting your new
standard, and then submitting a
[pull request](https://help.github.com/articles/using-pull-requests) to the
origin repository.

### [Adding an Extension]({{ site.baseurl }}/extensions/add.html)

An extension needs to reference an existing standard. Extensions are typically
enhancements to a standard that provide additional functionality or meet some
other requirements.

### [Adding a Tool]({{ site.baseurl }}/tools/add.html)

Tools are software tools or systems that support the use of the standard. Tools
implement the standard.

### [Adding a Use Case]({{ site.baseurl }}/use_cases/add.html)

Use cases are systems, organizations or projects which use the standard.

### Editing

Editing can take place within the GitHub editing tools. Or alternatively a fork
of the repository can be cloned and editing can be done locally and pull
requests can be generated using the existing GitHub and git workflows.

### Additional Help

[Creating and editing files in your repository](https://help.github.com/articles/creating-and-editing-files-in-your-repository)

[Collaboration on GitHub](https://help.github.com/categories/63/articles)

## Jekyll

The website is generated with [Jekyll](http://jekyllrb.com). The website uses
Jekyll to process HTML, YAML, and Markdown files to generate a static website.
