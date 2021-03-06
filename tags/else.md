---
layout: document
category: Tags
published: true
title: Else
description: The else tag is used within a containing conditional tag when the condition in the surrounding tag is not met.
tags:
  - Conditional tags
---

# Else

On this page:

* [Syntax](#syntax)
* [Attributes](#attributes)
* [Examples](#examples)

## Syntax

~~~ html
<txp:else />
~~~

The **else** tag is a *single* tag that is used within a containing conditional tag to provide the means to assign default, or alternative, behaviour when the condition in the surrounding tag is **not** met.

Visually, this is the general structure in which it is used:

~~~ html
<txp:if_conditional_tag>
    …Content if true…
<txp:else />
    …Content if not true…
</txp:if_conditional_tag>
~~~

## Attributes

This tag has no attributes.

## Examples

### Example 1: Display excerpt when available

~~~ html
<txp:if_excerpt>
    <txp:excerpt />
<txp:else />
    <txp:section link="1" />
</txp:if_excerpt>
~~~

When the excerpt is available it is displayed, but when it is missing a hyperlinked section name is displayed instead.

Other tags used: [excerpt](excerpt), [if_excerpt](if_excerpt), [section](section).
