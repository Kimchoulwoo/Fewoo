---
layout: default
work: true
main: true
title: "Blog"
description: 업로드 예정
main: true
project-header: false
---

<div class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.blogs == true %}

     {% include post-list.html %}

{% endif %}
{% endfor %}
</div>
