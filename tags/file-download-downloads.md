---
layout: document
category: tags
published: true
title: "File download downloads"
tags:
  - File tags
---

# File download downloads

On this page:

* [Syntax](#user-content-syntax)
* [Attributes](#user-content-attributes)
* [Examples](#user-content-examples)

## Syntax

```html
<txp:file_download_downloads />
```

The *file_download_downloads* tag is a __single__ tag that Textpattern will replace with the number of times the current file has been downloaded. Should be used in a Textpattern 'file' type @@Form template@@.

## Attributes

This tag has no attributes.

## Examples

### Example 1: Display the number of downloads

```html
<p>
    Downloads:
    <txp:file_download_downloads />
</p>