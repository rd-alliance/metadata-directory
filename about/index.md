---
slug: index
layout: about
title:  "Getting Started"
date:   2014-08-03 19:55:16
categories: jekyll update
---

## Structure of the Directory

Standards are contained within the
[`standards`]({{ site.repourl }}/tree/{{ site.repobranch }}/standards)
file system directory with each standard encoded into a markdown file with a
[YAML](http://en.wikipedia.org/wiki/YAML) preface. The YAML preface is
structured to encode the various elements describing a metadata standard or its
associated implementations. 

Implementations come in three different categories
[`extensions`]({{ site.repourl }}/tree/{{ site.repobranch }}/extensions),
[`tools`]({{ site.repourl }}/tree/{{ site.repobranch }}/tools),
and [`use_cases`]({{ site.repourl }}/tree/{{ site.repobranch }}/use_cases). Each grouping of
implementations are contained in their own file system directories.

Relationships between implementations and standards are created based on
recording related standards within each of the implementation metadata records.

## Getting Started 

[__Adding a Standard__]({{ site.baseurl }}/standards/add.html)

Adding a new standard is as simple as forking the repository creating a new
standards file marked up with a simple YAML schema. Commiting your new
standard, and then submitting a
[pull request](https://help.github.com/articles/using-pull-requests) to the
origin repository.

[__Adding an Extension__]({{ site.baseurl }}/extensions/add.html)

An extension needs to reference an existing standard. Extensions are typically
enhancements to a standard that provide additional functionality or meet some
other requirements.

[__Adding a Tool__]({{ site.baseurl }}/tools/add.html)

Tools are software tools or systems that support the use of the standard. Tools
implement the standard.

[__Adding a Use Case__]({{ site.baseurl }}/use_cases/add.html)

Use cases are systems, organizations or projects which use the standard.

## Editing

Editing can take place within the GitHub editing tools. Or alternatively a fork
of the repository can be cloned and editing can be done locally and pull
requests can be generated using the existing GitHub and git workflows.

Experimenting with different workflows for editing is encouraged!

### Additional Help

[Creating and editing files in your repository](https://help.github.com/articles/creating-and-editing-files-in-your-repository)

[Collaboration on GitHub](https://help.github.com/categories/63/articles)

## Jekyll

The website is generated with [Jekyll](http://jekyllrb.com). The website uses
Jekyll to process HTML, YAML, and Markdown files to generate a static website.

If you choose to clone the repository running a local version of Jekyll is
helpful for troubleshooting:
[https://help.github.com/articles/using-jekyll-with-pages](https://help.github.com/articles/using-jekyll-with-pages)

