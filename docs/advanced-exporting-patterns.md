---
layout: docs
title: Exporting Patterns | Pattern Lab
heading: Exporting Patterns
---

{% capture m %}

While the Pattern Lab website is great for design, iteration, alignment, and discussion - you may find yourself wanting to export whole pattern markup snippets into a different environment.

In Pattern Lab Node, `patternlab-config.json` has two properties that work together to export completed patterns for use elsewhere. To export, provide an array of patternPartials and an output directory. Pattern Lab Node doesn't ship with any patternPartials specified for export. The default directory,`'./pattern_exports/'`, is created inside the install directory. Here is an example with three patternPartials set.

```javascript
"patternExportPatternPartials": ["molecules-primary-nav", "organisms-header", "organisms-footer"],
"patternExportDirectory": "./pattern_exports/"
```

Couple this technique with exported CSS via tools like [grunt-contrib-copy](https://github.com/gruntjs/grunt-contrib-copy) to really make patterns portable.

<strong>The PHP version of Pattern Lab is being deprecated in favor of a new unified Pattern Lab core. <a href='./php/advanced-exporting-patterns'>The PHP docs for this topic can be viewed here.</a></strong>

{% endcapture %}
{{ m | markdownify }}
