---
layout: default
title: Internationalist Communist Library
language: en
---

<div class="nav">
  <a href="{{ site.baseurl }}/">🇬🇧 English</a> |
  <a href="{{ site.baseurl }}/pt/">🇧🇷 Português</a> |
  <a href="{{ site.baseurl }}/es/">🇪🇸 Español</a> |
  <a href="{{ site.baseurl }}/it/">🇮🇹 Italiano</a>
</div>

<h1>☭ Internationalist Communist Library ☭</h1>
<p style="text-align: center; font-size: 1.1em;">
  Welcome to the official shared library for the Internationalist Communist Discord server
</p>

<h2>Library Sections</h2>

{% assign lang_sections = site.sections | where: "language", "en" | sort: "order" %}

{% if lang_sections.size > 0 %}
  <ul>
    {% for section in lang_sections %}
      <li><a href="{{ site.baseurl }}{{ section.url }}">{{ section.title }}</a></li>
    {% endfor %}
  </ul>
{% else %}
  <p>No sections added yet. Use the <a href="{{ site.baseurl }}/admin/" target="_blank">Admin Panel</a> to create them.</p>
{% endif %}

<p style="text-align: center; margin-top: 60px; font-size: 1.1em;">
  <a href="{{ site.baseurl }}/admin/" target="_blank">🔧 Open Admin Panel (Moderators only)</a>
</p>
