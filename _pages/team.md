---
layout: single
permalink: /team/
classes: wide
author_profile: false
---

<div class="team-grid">
  {% for person in site.people %}
    <div class="team-member">
      <img src="{{ person.image }}" alt="{{ person.name }}">
      <div class="team-member-bio">
        <h3>{{ person.name }}, {{ person.position }}</h3>
        <div>{{ person.content | markdownify }}</div>
      </div>
    </div>
  {% endfor %}
</div>
