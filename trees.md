---
name: Trees
---
# Trees

Trees are terrific!

<!--snippet-->

## Seed Collection

The collection of tree seeds is an excellent and cost-effective way to learn about and propagate trees.

```mermaid
gantt
    dateFormat  YYYY-MM-DD
    title       Tree Seed Collection Calendar

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
### {{ tree.name }} - {{ tree.type }} ({{ tree.status }})
{{ tree.content | markdownify }}
{% endfor %}

## References

- [https://dnr.wisconsin.gov/sites/default/files/topic/TreePlanting/SeedCollectionTraining.pdf](https://dnr.wisconsin.gov/sites/default/files/topic/TreePlanting/SeedCollectionTraining.pdf)
- [https://www.dnr.state.mn.us/forestry/nursery/collecting-conifer-cone.html](https://www.dnr.state.mn.us/forestry/nursery/collecting-conifer-cone.html)
- [https://www.dnr.state.mn.us/forestry/nursery/collecting-deciduous-seed.html](https://www.dnr.state.mn.us/forestry/nursery/collecting-deciduous-seed.html)
- [https://en.wikipedia.org/wiki/Juglans_nigra](https://en.wikipedia.org/wiki/Juglans_nigra)
