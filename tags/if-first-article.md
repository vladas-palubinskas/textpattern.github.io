---
layout: document
category: tags
published: true
title: "If first article"
tags:
  - Article tags
  - Conditional tags
---

# If first article

On this page:

* [Syntax](#user-content-syntax)
* [Attributes](#user-content-attributes)
* [Examples](#user-content-examples)

## Syntax

```html
<txp:if_first_article>
```

The *if_first_article* tag is a _conditional_ tag and always used as an opening and closing pair, like this...

```html
<txp:if_first_article>
    ...conditional statement...
</txp:if_first_article>
```

The tag will execute the contained statements if the displayed article is the first in the currently displayed list. It will display in both single article and article list modes. Should be used in an Textpattern 'article' type @@Form template@@.

## Attributes

This tag has no attributes.

## Examples

### Example 1: Add a linked section by title

```html
<h3>
    <txp:permlink>
        <txp:title />
    </txp:permlink>
    |
    <txp:posted />
    by
    <txp:author />
    <txp:if_first_article>
        | Section:
        <txp:section link="1" title="1" />
    </txp:if_first_article>
</h3>
<txp:body />
<txp:comments_invite wraptag="p" />
```

Displays a link to the header of the first article in an article list.

Other tags used: "permlink":permlink, "title":title, "author":author, "posted":posted, "section":section, "body":body, "comments_invite":comments-invite.

### Example 2: Add a class to a list item

```html
<li<txp:if_first_article> class="first"</txp:if_first_article>>
    <txp:permlink>
        <txp:title />
    </txp:permlink>
</li>
```

Adds a CSS class to the first article in an article list.

Other tags used: "permlink":permlink, "title":title.