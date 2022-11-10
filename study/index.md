---
layout: default
work: true
main: true
title: "Study"
description: 공부에 도움되거나 개발에 참고한 사이트
main: true
project-header: false
---

<div class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.studys == true %}

     {% include study-list.html %}

{% endif %}
{% endfor %}
</div>
