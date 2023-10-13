---
title: Cover
layout: cover
order: 1
menu: false
toc: false
image: figures/horakova-poggi-02.jpg
classes:
  - masthead
outputs:
  - html
---

<div class="masthead_info remove-paragraph-indent">

{% for editor in publication.series_editors %}
- {{ editor | markdownify }}
{% endfor %}

**Getty Research Journal Editorial Board**
{{ publication.series_editorial_board | markdownify }}

</div>

{% backmatter %}

{% for person in publication.project_team %}
- {{ person | markdownify }}
{% endfor %}

{% endbackmatter %}