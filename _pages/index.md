---
layout: page
title: Home
id: home
permalink: /
---

# Welcome! 🌱

This is my notekeeping for various D&D sessions. Mainly used to share with fellow players.
Most of it is nowhere near complete or accurate. 

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  DM:<br>
  The Sea Men <span style="font-weight: bold">[[Session List]]</span><br>
  An adventure in Wildemount inspired by the second campaign of Critical Role. 
</p>

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  Player:<br>
  The COKL <span style="font-weight: bold">[[Session List COKL]]</span><br>
  An adventure in Astella playing a Human Warlock named [[Redeef]]. 
</p>

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  Player/DM:<br>
  Forgotten Exiles <span style="font-weight: bold">[[Session List Forgotten Exiles]]</span><br>
  An adventure following the guild members of the Forgotten Exiles. 
</p>

This digital garden template is free, open-source, and [available on GitHub here](https://github.com/maximevaillancourt/digital-garden-jekyll-template).

The easiest way to get started is to read this [step-by-step guide explaining how to set this up from scratch](https://maximevaillancourt.com/blog/setting-up-your-own-digital-garden-with-jekyll).

<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
