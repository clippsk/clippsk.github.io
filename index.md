# Table of Contents

{% assign chaps = site.pages
  | where_exp: "p", "p.path contains 'chapters/'"
  | sort_natural: "name" %}

{% for p in chaps %}
- [{{ p.title | default: p.name | replace: '.md','' }}]({{ p.url }})
{% endfor %}
