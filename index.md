---
layout: default
title: DROP
subtitle: by apehex
---
{% for drop in site.drops %}
<article class="container box style1 right">
    <a href="{{ drop.readme }}" class="image fit"><img src="{{ 'assets/images/drop_bouncing.svg' | absolute_url }}" alt="" width="64" height="64"/>{{ drop.water }}</a>
    <div class="inner">
        <header>
            <h2>{{ drop.name }}</h2>
        </header>
        {{ drop.drop | markdownify }}
    </div>
</article>
{% endfor %}