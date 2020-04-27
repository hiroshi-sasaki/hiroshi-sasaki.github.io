---
title: 発表論文
layout: default
permalink: /publications
---

### 国際会議論文（査読有）
{% for pub in site.data.publications-conference %}
- **{{ pub.title }}**
  {{ pub.authors }}
  {{ pub.venue }}, {{ pub.year }}. {% if pub.rate %}(acceptance rate: {{ pub.rate}}){% endif %} {% if pub.misc %}({{ pub.misc }}){% endif %} {% if pub.award %}<br>***<font color="{{ site.data.theme.highlight_color }}"><b>{{ pub.award }}</b></font>***{% endif %}
{% endfor %}

### 学術論文（査読有・英文）
{% for pub in site.data.publications-journal %}
- **{{ pub.title }}**
  {{ pub.authors }}
  {{ pub.venue }}, pp.{{ pub.pages }}, {{ pub.month }} {{ pub.year }}. {% if pub.misc %}({{ pub.misc }}){% endif %} {% if pub.award %}<br>***<font color="{{ site.data.theme.highlight_color }}"><b>{{ pub.award }}</b></font>***{% endif %}
{% endfor %}

### 学術論文（査読有・和文）
{% for pub in site.data.publications-journal-ja %}
- **{{ pub.title }}**
  {{ pub.authors }}
  {{ pub.venue }}，pp.{{ pub.pages }}，{{ pub.year }}年{{ pub.month }}月．{% if pub.award %}<br>***<font color="{{ site.data.theme.highlight_color }}"><b>{{ pub.award }}</b></font>***{% endif %}
{% endfor %}

### 国際ワークショップ論文（査読有）
{% for pub in site.data.publications-workshop %}
- **{{ pub.title }}**
  {{ pub.authors }}
  {{ pub.venue }}, {{ pub.year }}. {% if pub.rate %}(acceptance rate: {{ pub.rate}}){% endif %} {% if pub.misc %}({{ pub.misc }}){% endif %} {% if pub.award %}<br>***<font color="{{ site.data.theme.highlight_color }}"><b>{{ pub.award }}</b></font>***{% endif %}
{% endfor %}
