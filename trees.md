---
name: Tree Species
---
{% for tree in site.tree_species %}
  <h2>{{ tree.name }} - {{ tree.type }} ({{ tree.status }})</h2>
  <p>{{ tree.content | markdownify }}</p>
{% endfor %}
