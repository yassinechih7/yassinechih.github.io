---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
{% for issue in site.collections %}
  <li>
    <h6 class="post-meta">
      Issue {{ issue[1].label }}
      &mdash;
      {{ issue[1].date | date: "%b %-d, %Y" }}
    </h6>
    <h2>
      {{ issue[1].title }}
    </h2>
  </li>
{% endfor %}