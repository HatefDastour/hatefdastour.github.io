---
layout: archive
title: "Notes"
permalink: /notes/
author_profile: true
---

{% include base_path %}


{% for post in site.mynotes %}
  {% include archive-single.html %}
{% endfor %}