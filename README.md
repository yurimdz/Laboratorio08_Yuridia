# tv-shows

Proyecto del laboratorio 08. Busca series por nombre usando la API de TVMaze y muestra sus episodios agrupados por temporada, con colores según el rating de cada uno.

## Cómo correrlo

Necesitás un servidor local, no abre directo con doble clic porque usa módulos ES (`import/export`).

La forma más fácil es con la extensión **Live Server** de VS Code: clic derecho en `src/index.html` → *Open with Live Server*.

## Estructura

```
tv-shows/
├── src/
│   ├── index.html
│   ├── index.css
│   ├── index.js             # busca, llama a los módulos y renderiza
│   ├── services/
│   │   └── tvmaze.js        # todo lo que tiene que ver con la API
│   └── components/
│       └── shows.js         # funciones que arman el HTML
├── .gitignore
├── package.json
└── README.md
```

## API

Usa [TVMaze](https://www.tvmaze.com/api). No requiere key ni autenticación.

- Buscar por nombre: `api.tvmaze.com/search/shows?q=nombre`
- Datos de una serie: `api.tvmaze.com/shows/:id`
- Episodios: `api.tvmaze.com/shows/:id/episodes`