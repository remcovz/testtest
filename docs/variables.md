---
title: "Github Variables"
category: test
tags: test
layout: page
---

| Variable | Value |
| ------ | ------- |
{% for item in site.github -%}
| {{ item[0] }} | {{ item[1] }} |
{% endfor %}
