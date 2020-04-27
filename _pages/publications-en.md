---
title: Publications
layout: default-en
permalink: /publications-en
---

### Conference Papers
{% for pub in site.data.publications-conference %}
- **{{ pub.title }}**
  {{ pub.authors }}
  {{ pub.venue }}, {{ pub.year }}. {% if pub.rate %}(acceptance rate: {{ pub.rate}}){% endif %} {% if pub.misc %}({{ pub.misc }}){% endif %} {% if pub.award %}<br>***<font color="{{ site.data.theme.highlight_color }}"><b>{{ pub.award }}</b></font>***{% endif %}
{% endfor %}

### Workshop Papers
{% for pub in site.data.publications-workshop %}
- **{{ pub.title }}**
  {{ pub.authors }}
  {{ pub.venue }}, {{ pub.year }}. {% if pub.rate %}(acceptance rate: {{ pub.rate}}){% endif %} {% if pub.misc %}({{ pub.misc }}){% endif %} {% if pub.award %}<br>***<font color="{{ site.data.theme.highlight_color }}"><b>{{ pub.award }}</b></font>***{% endif %}
{% endfor %}

### Journal Papers
{% for pub in site.data.publications-journal %}
- **{{ pub.title }}**
  {{ pub.authors }}
  {{ pub.venue }}, pp.{{ pub.pages }}, {{ pub.month }} {{ pub.year }}. {% if pub.misc %}({{ pub.misc }}){% endif %} {% if pub.award %}<br>***<font color="{{ site.data.theme.highlight_color }}"><b>{{ pub.award }}</b></font>***{% endif %}
{% endfor %}
