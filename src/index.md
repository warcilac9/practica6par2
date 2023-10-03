---
layout: base.njk
title: Wilbert Arcila Castellanos 
---

# {{ title }}

[Acerca]({{ '/acerca' | url }})

## Artículos

### Animes:

{% for libro in collections.libros %}

- [{{libro.data.title}}]({{ libro.url | url }})

{% endfor %}

### Videojuegos

{% for serie in collections.series %}

- [{{serie.data.title}}]({{ serie.url | url }})

{% endfor %}

### Peliculas

{% for peli in collections.peliculas %}

- [{{peli.data.title}}]({{peli.url | url}})

{% endfor %}
