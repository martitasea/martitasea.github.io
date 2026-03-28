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
  - type: list
    name: Vista
    filters:
      and:
        - categorias.contains(link("Recetas"))

```



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
  - type: list
    name: Vista
    filters:
      and:
        - categorias.contains(link("Recetas"))

```

