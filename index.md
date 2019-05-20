---
layout: default
title: DROP
subtitle: by apehex
---
{% for drop in site.drops %}
<article class="container box style4 right">
    <a href="{{ drop.url }}">
        <div class="upper">
            <header>
                <h2>{{ drop.name }}</h2>
            </header>
            {{ drop.drop | markdownify }}
        </div>
        <div class="lower">
            {{ drop.water | markdownify }}
        </div>
    </a>
</article>
{% endfor %}