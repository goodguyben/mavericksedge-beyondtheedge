---
layout: default
title: Home
---

# {{ site.title }}

{{ site.description }}

## Recent Posts

<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    — {{ post.date | date: "%Y-%m-%d" }}
    {% if post.excerpt %}
    <br><small>{{ post.excerpt }}</small>
    {% endif %}
  </li>
{% endfor %}
</ul>

---

*Powered by [Mavericks Edge](https://mavericksedge.ca) - Edmonton's premier web design agency*
