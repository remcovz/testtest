---
title: "Collections Demo"
date: 2018-05-14 00:10:00 +0200
category: collections
tags: [test, collections]
layout: post
---
{% for album in site.albums %}
  <h2>{{ album.title }}</h2>
  <p>Performed by {{ album.artist }}{% if album.director %}, directed by {{ album.director }}{% endif %}</p>
  {% for work in album.works %}
    <h3>{{ work.title }}</h3>
    <p>Composed by {{ work.composer }}</p>
    <ul>
    {% for track in work.tracks %}
      <li>{{ track.title }} ({{ track.duration }})</li>
    {% endfor %}
    </ul>
  {% endfor %}
{% endfor %}

