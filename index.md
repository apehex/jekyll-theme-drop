---
layout: default
title: DROP
subtitle: by apehex
---
{% for drop in site.drops %}
<article class="container box style4 right">
    <a href="{{ drop.url }}">
        <div class="upper">
            {% include bouncing.svg width="360px" height="60px" view-box="220 0 140 60" fill="#182d3a" opacity="1" %}
            <div class="inner">
                <header>
                    <h2>{{ drop.name }}</h2>
                </header>
                {{ drop.drop | markdownify }}
            </div>
        </div>
        <div class="lower">
            {% include bouncing.svg width="360px" height="60px" view-box="220 60 140 60" fill="#00ffff" opacity="1" %}
            <div class="inner">
                {{ drop.water | markdownify }}
            </div>
        </div>
    </a>
</article>
{% endfor %}