---
layout: document
category: Tags
published: true
title: If article list
description: The if_article_list tag will execute the contained statement if an article list is being displayed.
tags:
  - Article tags
  - Conditional tags
---

# If article list

On this page:

* [Syntax](#syntax)
* [Attributes](#attributes)
* [Examples](#examples)
* [Genealogy](#genealogy)

## Syntax

~~~ html
<txp:if_article_list>
~~~

The **if_article_list** tag is a *conditional* tag and always used as an opening and closing pair, like this…

~~~ html
<txp:if_article_list>
    …conditional statement…
</txp:if_article_list>
~~~

The tag will execute the contained statement if an article list is being displayed (i.e. not showing an individual article).

## Attributes

Tag will accept the following attributes (**case-sensitive**):

`type="list"` <span class="footnote warning">v4.7.0+</span>
: Check whether some of Textpattern’s filters are set.
: **Values:** a comma-separated list of `author, c, context, month, pg, q, s`.
: **Default:** unset.

## Examples

### Example 1: Article/article list navigation

~~~ html
<txp:article />

<txp:if_individual_article>
    <p>
        <txp:link_to_prev>
            <txp:prev_title />
        </txp:link_to_prev>
        <txp:link_to_next>
            <txp:next_title />
        </txp:link_to_next>
    </p>
</txp:if_individual_article>

<txp:if_article_list>
    <p>
        <txp:older>Previous</txp:older>
        <txp:newer>Next</txp:newer>
    </p>
</txp:if_article_list>
~~~

This example shows how to setup article navigation so that [link_to_prev](link_to_prev) and [link_to_next](link_to_next) are used at the individual article level *or* [older](older) and [newer](newer) with article lists.

Other tags used: [link_to_prev](link_to_prev), [link_to_next](link_to_next), [prev_title](prev_title), [next_title](next_title), [if_individual_article](if_individual_article), [older](older), [newer](newer).

### Example 2: In combination with the 'else' tag

~~~ html
<txp:if_article_list>
    <p>
        <txp:site_name />
    </p>
<txp:else />
    <p>
        <img src="http://example.com/logo.png" alt="Logo">
    </p>
</txp:if_article_list>
~~~

This example shows the if_article_list in combination with [else](else) to display a site's [site_name](site_name) or logo when an article list is displayed or not, respectively.

Other tags used: [else](else), [site_name](site_name).

## Genealogy

### Version 4.7.0

`type` attribute added.
