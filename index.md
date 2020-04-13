---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

<h1 class="page-heading mb-5">Nýjustu færslur</h1>

<ul class="post-list list-unstyled">
  {% for post in site.posts %}
    <li class="my-5">

      <div class="post-header text-center mb-3">
        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
        <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
      </div>
      <p>{{ post.content | strip_html | truncatewords: 80 }}</p>
      <div class="text-center">
        <a class="btn btn-outline-primary" href="{{ post.url }}">Lesa meira</a><br><br>
      </div>

    </li>
  {% endfor %}
</ul>
