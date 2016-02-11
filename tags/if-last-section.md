---
layout: document
category: tags
published: true
title: "If last section"
tags:
  - Conditional tags
  - Structural tags
---

# If last section

On this page:

* [Syntax](#user-content-syntax)
* [Attributes](#user-content-attributes)
* [Examples](#user-content-examples)
* [Genealogy](#user-content-genealogy)

## Syntax

```html
<txp:if_last_section>
```

The *if_last_section* tag is a _conditional_ tag and always used as an opening and closing pair, like this...

```html
<txp:if_last_section>
    ...conditional statements...
</txp:if_last_section>
```

The tag will execute the contained statements if the current section (usually one inside the container or form of a "section_list":/section-list) is the last in the currently displayed list.

## Attributes

This tag has no attributes.

## Examples

### Example 1: Assign a specific id to the last item in the list

```html
<txp:section_list wraptag="ul" break="">
    <li<txp:if_last_section> id="last"</txp:if_last_section>>
        <txp:section title="1" link="1" />
    </li>
</txp:section_list>
```

## Genealogy

### Version 4.0.7

Tag support added.