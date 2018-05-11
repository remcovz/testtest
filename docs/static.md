---
layout: page
title: Static files
---
{% for asset in site.static_files %}
  File: {{ asset.path }}<br>
  Modified_time: {{ asset.modified_time }}<br>
  name: {{ asset.time }}<br>
  basename: {{ asset.basename }}<br>
  extname: {{ asset.extname }}<br>
{% endfor %}
