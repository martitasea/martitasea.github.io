---
{"dg-publish":true,"permalink":"/categorias/recetas/","tags":["categorias","gardenEntry"],"dg-note-properties":{"tags":["categorias","gardenEntry"]}}
---


```base
filters:
  and:
    - '!file.name.contains("Plantilla")'
    - file.folder == "Referencias"
views:
  - type: table
    name: Recetas
    filters:
      or:
        - categorias.contains("Recetas")
        - categorias.contains(link("Categorías/Recetas"))
    order:
      - dg-publish
      - file.name
      - autor
      - cocina
      - tipo
      - raciones
      - dificultad
      - tiempo (min)
      - url
    columnSize:
      file.name: 142

```


[[Referencias/Albondigón Frío\|Albondigón Frío]]
[[Referencias/Brownie\|Brownie]]
[[Referencias/Caldo de verduras\|Caldo de verduras]]
[[Referencias/Gazpacho\|Gazpacho]]
[[Referencias/Lentejas estofadas\|Lentejas estofadas]]
[[Referencias/Pote gallego\|Pote gallego]]
[[Referencias/Salsa romescu\|Salsa romescu]]
