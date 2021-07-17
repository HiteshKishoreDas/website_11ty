---
layout: base.liquid
---

# I'm making upgrades to my site!

For the old website, visit [(hiteshkishoredas.github.io)].
This new website will take sometime to get built as I'm still the ropes of static site generators.

{% for post in collections.posts reversed %}
  <a href="{{ post.url }}">
    <h2>{{ post.data.title }}</h2>
    <time>{{ post.data.date | date: "%B %d, %Y" }}</time>
  </a>
{% endfor %}
