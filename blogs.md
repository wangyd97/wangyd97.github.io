---
layout: page
permalink: /blogs/index.html
title: Blogs
---

## Blogs 博客

### 2025

<ul>
{% for item in site.pages %}
  {% if item.url contains '/blogs/' and item.url != '/blogs/index.html' %} 
    {% if item.date %}
      {% if item.date | date: "%Y" == "2025" %}
        <li>
          <a href="{{ item.url }}">{{ item.title }}</a><br>
        </li>
      {% endif %}
    {% endif %}
  {% endif %}
{% endfor %}
</ul>

<br>


<br>

## Leave a Message 欢迎留言

{% include disqus.html %} 

<br>

Finally, my WeChat account is - **cwjykdk*

<br>
