# Dev Microtools

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Deployed-2ea44f?logo=github)](https://ailtonbsj.github.io/dev-microtools/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)
[![Made with HTML5](https://img.shields.io/badge/Made%20with-HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/docs/Web/HTML)
[![Made with CSS3](https://img.shields.io/badge/Made%20with-CSS3-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/docs/Web/CSS)
[![Made with JavaScript](https://img.shields.io/badge/Made%20with-JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/docs/Web/JavaScript)

**Languages:** [English](./README.md) · [Português (Brasil)](./README.pt-BR.md)

A collection of browser-based microtools for everyday development tasks, focused on **Java/Spring** and **Angular/TypeScript**.

🔗 **Demo:** [ailtonbsj.github.io/dev-microtools](https://ailtonbsj.github.io/dev-microtools/)

## Overview

This repository brings together simple tools that run directly in the browser to speed up common development tasks (conversions, boilerplate generation, and code transformations).

The project consists of:
- a **web catalog** (`index.html`) to search, filter, and open tools;
- **local tools** versioned in this repository (self-contained HTML files);
- references to **external tools** maintained within the same ecosystem.

## Tools in the catalog

| Tool | Description | Tags | Catalog preview |
|---|---|---|---|
| [Java DTO to Angular Model](https://ailtonbsj.github.io/dev-microtools/java-dto-to-ts.html) | Converts Java DTO classes into TypeScript interfaces (parser based on `java-ast`) | `frontend`, `angular`, `backend`, `java` | Yes |
| [Constructor to Inject Angular](https://ailtonbsj.github.io/dev-microtools/angular-constructor-to-inject.html) | Converts Angular constructor-based dependency injection to `inject()` | `frontend`, `angular` | Yes |
| [SQL CREATE to Spring/Angular Boilerplate](https://dev-tools-converters.vercel.app/ddl-to-module/) | Generates Spring Boot and Angular boilerplate from `CREATE TABLE` statements | `frontend`, `backend`, `sql`, `spring`, `angular` | No |
| [JSON to SQL for Oracle DB](https://ailtonbsj.github.io/json-to-sql/) | Converts DBeaver-exported JSON into SQL for Oracle DB | `backend`, `sql`, `dbeaver` | Yes |
| [PDF Region Generator for PDFBox Java](https://ailtonbsj.github.io/pdf-region-generator/) | Generates Java snippets with PDF regions for PDFBox | `backend`, `java`, `pdfbox` | Yes |
| [ENV to JSON Converter](https://ailtonbsj.github.io/env-to-json/) | Converts between `.env` and JSON | `backend`, `spring`, `java` | Yes |

> The list above reflects the catalog defined in `index.html`. External tools may be hosted in other repositories/domains.

## Local tools (in this repository)

- `index.html` — Microtools catalog/launcher with search by name, tag filtering, card/table view, and embedded preview (iframe) when enabled.
- `java-dto-to-ts.html` — Converts a Java DTO class into a TypeScript interface.
- `angular-constructor-to-inject.html` — Converts Angular constructor injection into the `inject()` API.

## Catalog features

- Search tools by name
- Filter by tags
- Switch between **card** and **table** views
- Open in a new tab
- Embedded preview for tools with `preview: true`

## Running locally

Since this is a static project (HTML/CSS/JS), you can open the files directly in your browser or serve the folder with a simple HTTP server.

### Option 1: Open directly
Open `index.html` in your browser.

### Option 2: Local server (recommended)

```bash
# from the project root
python3 -m http.server 8000
```

Then visit: `http://localhost:8000`

## Adding a new tool to the catalog

Edit the `tools` array in `index.html` and add a new object with the following fields:

```js
{
  name: 'Tool name',
  description: 'Short description',
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