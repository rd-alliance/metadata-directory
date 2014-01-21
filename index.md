---
title: Metadata Directory
type: home
layout: base

---

Prototype metadata directory for the Research Data Alliance

## Instructions


[Creating and editing files in your repository](https://help.github.com/articles/creating-and-editing-files-in-your-repository)

adding a file:
:  https://github.com/{user}/{project}/new/{branch}{/directory}?filename={filename}

editing a file
:  https://github.com/{user}/{project}/edit/{branch}/{filename}

## Standards

[Visit the standards]({{ site.baseurl }}/standards/)

adding a new standard:
:  https://github.com/{user}/{project}/new/{branch}{/directory}?filename={filename}.md

Data should be laid out in a
[markdown](http://daringfireball.net/projects/markdown/syntax) file with a
[YAML](http://www.yaml.org/) preface.

    ---
    title: {Title of the Standard}
    name: {Short name for references}
    layout: standard
    type: standard
    subjects:
      - { values of subjects }
    specification_url: http://url.to.specification
    website: http://url.to.project.website
    related_vocabularies:
      -
        name: {name of related vocabulary}
        url: {url of related vocabulary}
      -
        name: {second name of related vocabulary}
        url: {url of second related vocabulary}
    mappings:
      -
        name: {name of metadata mapping}
        url: {url of mapping}
      -
        name: {second name of metadata mapping}
        url: {second url of mappings}
    sponsor: {Sponsoring organization}
    update: {update date ISO date format}
    version: {version data }
    description: |
      { two sentence summary }
    ---

## Extensions

[Visit the extensions]({{ site.baseurl }}/extensions/)

## Tools

[Visit the tools]({{ site.baseurl }}/tools/)

## Use Cases

[Visit the use cases]({{ site.baseurl}}/use_cases/)

## Directory Structure

    .
    ├── _layouts
    |   └── base.html
    ├── js
    |   └── bootstrap.min.js
    ├── css
    |   └── bootstrap.min.css
    |
    ├── images
    |
    ├── standards
    |   └── standard_name.md
    ├── extensions
    |   └── extension_name.md
    ├── tools
    |   └── tool_name.md
    ├── use_cases
    |   └── use_case_name.md
    └── index.md
