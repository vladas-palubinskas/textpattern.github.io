---
layout: document
category: tags
published: true
title: "Title"
tags:
  - Article tags
---

# Title

On this page:

* [Syntax](#user-content-syntax)
* [Attributes](#user-content-attributes)
* [Examples](#user-content-examples)

## Syntax

```html
<txp:title />
```

The *title* tag is a __single__ tag which is used to return the title of the article being displayed. It is usually used in an 'article' type form.

## Attributes

Tag will accept the following attributes (**case-sensitive**):

* @no_widow="boolean"@
Control "widows":http://en.wikipedia.org/wiki/Widows_and_orphans and overrule 'widows' setting in the "Preferences administration panel":http://docs.textpattern.io/administration/preferences-panel.
Values: `0` allow the last word in the title to appear on its own line, i.e. the title content is rendered unchanged, `1` ensure the last word is not left on its own line - Textpattern inserts an invisible code (a non-breaking space) between the last two words.
Default: as set in the "Preferences administration panel":http://docs.textpattern.io/administration/preferences-panel.

## Examples

### Example 1: Display an article title

```html
<h1>
    <txp:title />
</h1>
<p>
    <txp:author /> at <txp:posted />
</p>
<txp:body />
```

Shows the current article title as the page heading, a few other pieces of information such as the article's author and posted date, then the article body itself.

Other tags used: "author":http://docs.textpattern.io/tags/author, "posted":http://docs.textpattern.io/tags/posted, "body":http://docs.textpattern.io/tags/body.

### Example 2: Display a hyperlinked title

```html
<txp:permlink>
    <txp:title />
</txp:permlink>
```

Wraps a permanent link to the current article around its title.

Other tags used: "permlink":http://docs.textpattern.io/tags/permlink.