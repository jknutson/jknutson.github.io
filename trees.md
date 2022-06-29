---
name: Trees
---
# Trees

Trees are neat.

<!--snippet-->

## Seedling Collection

Collecting Tree Seedlings is an excellent and cost-effective way to learn about and propagate trees!

```mermaid
gantt
    dateFormat  YYYY-MM-DD
    title       Tree Seedling Collection Calendar

    section Basswood (Linden)
    Scout Seeds         :ldn1, 2022-06-20, 40d
    Collect Seeds       :ldn2, 2022-09-01, 120d

    section Black Walnut
    Scout Seeds         :bw1, 2022-07-01, 30d
    Collect Seeds       :bw2, 2022-10-01, 30d

    section White Spruce
    Scout Seeds         :ws1, 2022-06-01, 30d
    Collect Seeds       :ws2, 2022-08-20, 40d

```

## Species

{% for tree in site.tree_species %}
  <h2>{{ tree.name }} - {{ tree.type }} ({{ tree.status }})</h2>
  <p>{{ tree.content | markdownify }}</p>
{% endfor %}

## References

- https://dnr.wisconsin.gov/sites/default/files/topic/TreePlanting/SeedCollectionTraining.pdf
- https://www.dnr.state.mn.us/forestry/nursery/collecting-conifer-cone.html
- https://www.dnr.state.mn.us/forestry/nursery/collecting-deciduous-seed.html
