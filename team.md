---
layout: page
title: Team
subtitle: Alle jene, die für die Organisation unserer LoL-Turniere verantworlich sind.
---

<div class="team">
  {% for member in site.data.team %}
  {% capture link %}https://gamekeller.net/{% if member.account %}{{ member.account }}{% else %}{{ member.name }}{% endif %}{% endcapture %}
  <a class="team-person" href="{{ link }}" target="_blank">
    <img class="team-person-avatar" src="{{ link }}/avatar">
    <p class="team-person-name">{{ member.name }}</p>
  </a>
  {% endfor %}
</div>