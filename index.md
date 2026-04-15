---
layout: default
title: Internationalist Communist Library
language: en
---

<div class="nav">
  <a href="{{ site.baseurl }}/">🇬🇧 English</a> |
  <a href="{{ site.baseurl }}/pt/">🇧🇷 Português</a> |
  <a href="{{ site.baseurl }}/es/">🇪🇸 Español</a> |
  <a href="{{ site.baseurl }}/it/">🇮🇹 Italiano</a> |
  <a href="{{ site.baseurl }}/nl/">🇳🇱 Nederlands</a> |
  <a href="{{ site.baseurl }}/de/">🇩🇪 Deutsch</a> |
  <a href="{{ site.baseurl }}/el/">🇬🇷 Ελληνικά</a>
</div>

<h1>☭ Internationalist Communist Library ☭</h1>
<p style="text-align: center; font-size: 1.1em;">
  Welcome to the official shared library for the Internationalist Communist Discord server
</p>

<h2>Library Sections</h2>

{% assign lang_sections = site.sections | where: "language", "en" | sort: "order" %}

{% for section in lang_sections %}
  <div style="margin: 25px 0; padding: 20px; border-left: 5px solid #e63939; background: #2d2d2d;">
    <h3><a href="{{ site.baseurl }}{{ section.url }}">{{ section.title }}</a></h3>
    {{ section.content | markdownify | truncatewords: 60 }}
    <p style="margin-top: 15px;">
      <a href="{{ site.baseurl }}{{ section.url }}">→ Read full section</a>
    </p>
  </div>
{% endfor %}

<p style="text-align: center; margin-top: 70px;">
  <a href="{{ site.baseurl }}/admin/" target="_blank">🔧 Open Admin Panel (Moderators only)</a>
</p>---
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
  <strong>Welcome to the official shared library for the Internationalist Communist Discord server</strong>
</p>

<h2>Library Sections</h2>

{% assign lang_sections = site.sections | where: "language", "en" | sort: "order" %}

{% for section in lang_sections %}
  <div style="margin: 25px 0; padding: 20px; border-left: 5px solid #e63939; background: #2d2d2d;">
    <h3><a href="{{ site.baseurl }}{{ section.url }}">{{ section.title }}</a></h3>
    {{ section.content | markdownify | truncatewords: 60 }}
    <p style="margin-top: 15px;">
      <a href="{{ site.baseurl }}{{ section.url }}">→ Read full section</a>
    </p>
  </div>
{% endfor %}

<p style="text-align: center; margin-top: 70px; font-size: 1.1em;">
  <a href="{{ site.baseurl }}/admin/" target="_blank">🔧 Open Admin Panel (Moderators only)</a>
</p>
