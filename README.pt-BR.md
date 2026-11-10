# Dev Microtools

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Deployed-2ea44f?logo=github)](https://ailtonbsj.github.io/dev-microtools/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)
[![Made with HTML5](https://img.shields.io/badge/Made%20with-HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/docs/Web/HTML)
[![Made with CSS3](https://img.shields.io/badge/Made%20with-CSS3-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/docs/Web/CSS)
[![Made with JavaScript](https://img.shields.io/badge/Made%20with-JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/docs/Web/JavaScript)

**Idiomas:** [English](./README.md) · [Português (Brasil)](./README.pt-BR.md)

Coleção de microferramentas para o dia a dia de desenvolvimento, com foco em **Java/Spring** e **Angular/TypeScript**.

🔗 **Page:** [ailtonbsj.github.io/dev-microtools](https://ailtonbsj.github.io/dev-microtools/)

## Visão geral

Este repositório reúne ferramentas simples, executadas diretamente no navegador, para acelerar tarefas comuns de desenvolvimento (conversões, geração de boilerplate e transformações de código).

O projeto é composto por:
- um **catálogo web** (`index.html`) para buscar, filtrar e abrir as ferramentas;
- **ferramentas locais** versionadas neste repositório (arquivos HTML autocontidos);
- referências a **ferramentas externas** mantidas pelo mesmo ecossistema.

## Funcionalidades do catálogo

- Busca por nome da ferramenta
- Filtro por tags
- Alternância entre visualização em **cards** e **tabela**
- Abertura em nova aba
- Visualização embarcada (preview) para ferramentas com `preview: true`

## Como adicionar uma nova ferramenta ao catálogo

Edite o array `tools` em `index.html` e inclua um novo objeto com os campos:

```js
{
  name: 'Nome da ferramenta',
  description: 'Descrição curta',
  url: 'https://exemplo.com/ferramenta',
  tags: ['tag1', 'tag2'],
  authors: ['autor'],
  preview: true // ou false
}
```

- `preview: true` habilita o botão de visualização embarcada no catálogo (quando aplicável/permitido pelo destino).

## Tecnologias

- HTML, CSS e JavaScript (vanilla)
- Hospedagem estática (compatível com GitHub Pages)
- Sem etapa de build obrigatória

## Licença

Este projeto está licenciado sob a [MIT License](./LICENSE).