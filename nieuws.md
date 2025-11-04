---
layout: page
title: "Nieuws"
subtitle: "Blijf op de hoogte van onze activiteiten"
description: "Nieuws en updates van Brassband Eensgezindheid Wormer"
---

## Laatste Nieuws

Hier vindt u het laatste nieuws over onze brassband, optredens, en activiteiten.

{% for post in site.posts %}
<article class="news-item">
  <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
  <p class="news-meta">{{ post.date | date: "%d %B %Y" }}</p>
  {% if post.excerpt %}
  <p>{{ post.excerpt }}</p>
  {% endif %}
  <a href="{{ post.url | relative_url }}" class="btn btn--secondary">Lees meer →</a>
</article>
{% endfor %}

{% if site.posts.size == 0 %}
<p>Er zijn momenteel geen nieuwsberichten. Houd deze pagina in de gaten voor updates!</p>
{% endif %}

## Blijf op de hoogte

Wilt u automatisch op de hoogte blijven van ons nieuws? Schrijf u dan in voor onze nieuwsbrief via de [contact pagina](/contact/#newsletter).