---
layout: collection
category: Tags
published: true
title: "Category: Programmer tags"
description: A list of Textpattern documentation within the category 'Programmer tags'.
search_omit: true
---

# Category: Programmer tags

Textpattern documentation within the category 'Programmer tags':

<ol class="list--no-bullets">
    {% for page in site.pages %}
        {% if page.tags contains 'Programmer tags' %}
            {% include article-listing.html %}
        {% endif %}
    {% endfor %}
</ol>
