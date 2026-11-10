# Dev Microtools

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Deployed-2ea44f?logo=github)](https://ailtonbsj.github.io/dev-microtools/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)
[![Made with HTML5](https://img.shields.io/badge/Made%20with-HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/docs/Web/HTML)
[![Made with CSS3](https://img.shields.io/badge/Made%20with-CSS3-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/docs/Web/CSS)
[![Made with JavaScript](https://img.shields.io/badge/Made%20with-JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/docs/Web/JavaScript)

**Languages:** [English](./README.md) · [Português (Brasil)](./README.pt-BR.md)

A collection of browser-based microtools for everyday development tasks, focused on **Java/Spring** and **Angular/TypeScript**.

🔗 **Page:** [ailtonbsj.github.io/dev-microtools](https://ailtonbsj.github.io/dev-microtools/)

## Overview

This repository brings together simple tools that run directly in the browser to speed up common development tasks (conversions, boilerplate generation, and code transformations).

The project consists of:
- a **web catalog** (`index.html`) to search, filter, and open tools;
- **local tools** versioned in this repository (self-contained HTML files);
- references to **external tools** maintained within the same ecosystem.

## Catalog features

- Search tools by name
- Filter by tags
- Switch between **card** and **table** views
- Open in a new tab
- Embedded preview for tools with `preview: true`

## Adding a new tool to the catalog

Edit the `tools` array in `index.html` and add a new object with the following fields:

```js
{
  namePtBr: 'Nome da ferramenta',
  nameEn: 'Tool name',
  descriptionPtBr: 'Descrição curta',
  descriptionEn: 'Short description',
  url: 'https://example.com/tool',
  tags: ['tag1', 'tag2'],
  authors: ['author'],
  preview: true // or false
}
```

- `preview: true` enables the embedded preview button in the catalog (when applicable/allowed by the target).

## Technologies

- HTML, CSS, and JavaScript (vanilla)
- Static hosting (compatible with GitHub Pages)
- No mandatory build step

## License

This project is licensed under the [MIT License](./LICENSE).
