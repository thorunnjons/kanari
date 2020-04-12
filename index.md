---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

<h1 class="page-heading">Nýjustu færslur</h1>

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
      <i>{{ post.content | strip_html | truncatewords: 80 }}</i><br>
      <a href="{{ post.url }}">Read more...</a><br><br>

    </li>
  {% endfor %}
</ul>
