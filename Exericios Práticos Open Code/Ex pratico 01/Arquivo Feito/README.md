# Café Aurora ☕

Projeto prático desenvolvido exclusivamente com **HTML5** e **CSS3**, sem JavaScript, frameworks, bibliotecas CSS, Flexbox ou CSS Grid.

## 1. Objetivo do projeto

Este projeto simula o site institucional de uma cafeteria artesanal fictícia chamada **Café Aurora**. Ele foi criado como exercício prático para consolidar conceitos de HTML5 semântico e CSS3 "tradicional" (baseado em `position`, `display`, seletores, pseudo-classes e pseudo-elementos), sem recorrer a Flexbox, Grid ou JavaScript.

A ideia é que o site sirva como **referência visual pronta**: explore-o no navegador, inspecione o código-fonte e, depois, tente recriá-lo do zero utilizando apenas os conhecimentos que já estudou. Só depois compare o seu resultado com este projeto original.

## 2. Como abrir o projeto

Não é necessário nenhum servidor ou instalação:

1. Extraia/abra a pasta `cafe-aurora`.
2. Dê duplo clique no arquivo `index.html` (ou abra-o com o navegador da sua preferência).
3. Navegue pelas seções usando o menu do cabeçalho.

> O projeto funciona 100% localmente. As únicas dependências externas são a fonte do Google Fonts e algumas imagens hospedadas no Unsplash (ver seção 6).

## 3. Estrutura de arquivos

```
cafe-aurora/
│
├── index.html          → Estrutura HTML5 completa do site
├── style.css            → Toda a estilização do projeto
├── README.md             → Este arquivo
│
├── imagens/
│   └── favicon.svg      → Ícone do site
│
├── audio/
│   └── (adicione aqui um arquivo ambiente-cafe-aurora.mp3, se desejar)
│
└── fontes/
    └── (pasta reservada — as fontes utilizadas vêm do Google Fonts via @import)
```

## 4. Conceitos de HTML5 utilizados

- Estrutura semântica: `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>`
- Textos e ênfase: `<h1>` a `<h3>`, `<p>`, `<strong>`, `<em>`, `<mark>`, `<small>`, `<abbr>`, `<blockquote>`, `<hr>`, `<sub>`, `<sup>`
- Listas: `<ul>`, `<ol>`, `<li>`, `<dl>`, `<dt>`, `<dd>`
- Tabelas: `<table>`, `<tr>`, `<th>`, `<td>`
- Mídia responsiva: `<picture>`, `<source>`, `<img>` (com `srcset`/`media`)
- Mídia incorporada: `<audio controls>` e `<iframe>` (vídeo do YouTube)
- Código: `<pre>`, `<code>`
- Formulário: `<form>`, `<label>`, `<input>` (text, email, checkbox), `<select>`, `<option>`, `<textarea>`, `<button>`
- Entidades HTML: `&copy;`, `&reg;`

## 5. Conceitos de CSS3 utilizados

- Variáveis CSS em `:root` (cores e fontes)
- Seletores de tag, classe, ID, universal e de filho direto
- Pseudo-classes: `:hover`, `:visited`, `:active`, `:focus`, `:checked`, `:empty`
- Pseudo-elementos: `::before`, `::after`, `::first-letter`, `::first-line`
- `linear-gradient` para fundos (cabeçalho e banner promocional)
- `text-shadow`, `box-shadow`, `border-radius`
- `position: relative` + `position: absolute` (etiqueta "Mais Vendido" e vídeo responsivo)
- `columns` para dividir listas em colunas
- `@import` para fonte externa (Google Fonts)
- `@media` para responsividade (tablet e smartphone)
- `box-sizing: border-box` (ver observação abaixo)

### Observação sobre `box-sizing: border-box`

O projeto utiliza `box-sizing: border-box` no reset global (`*`). Essa propriedade foi incluída porque simplifica bastante o cálculo de larguras quando `padding` e `border` são usados em conjunto com `width: 100%` — o que evita que elementos "estourem" a largura do contêiner, algo comum quando não se utiliza Flexbox ou Grid para organizar o layout.

## 6. Onde cada conceito aparece

| Conceito | Onde encontrar |
|---|---|
| `::first-letter` / `::first-line` | Seção "Nossa História" |
| `<picture>` + `srcset`/`media` | Seção "Nossa Origem" |
| `columns` | Lista de bebidas, seção "Cardápio" |
| `<dl>`/`<dt>`/`<dd>` | Glossário, seção "Cardápio" |
| Tabela estilizada | Seção "Tabela de Produtos" |
| `position: relative/absolute` (vídeo) | Seção "Experiência Café Aurora" |
| `<audio>` e `<iframe>` | Seção "Experiência Café Aurora" |
| `<aside>` com `::before` | Seção "Curiosidades" |
| `<sub>`/`<sup>`/`<pre>`/`<code>` | Seção "Você Sabia?" |
| `linear-gradient` + `::before`/`::after` decorativos | Banner "Semana do Café Especial" |
| `:empty` | `<div class="decoracao">` logo após o banner |
| `:checked`, `:focus`, `:hover` no formulário | Seção "Fale Connosco" |
| Entidades HTML `&copy;`/`&reg;` | Rodapé |

## Sobre os recursos externos utilizados

- **Fontes**: "Playfair Display" e "Poppins", carregadas via `@import` do Google Fonts.
- **Imagens**: fotografias de café hospedadas no Unsplash (URLs públicas), usadas apenas para fins ilustrativos.
- **Áudio**: o elemento `<audio>` aponta para `audio/ambiente-cafe-aurora.mp3`, mas nenhum arquivo de áudio real foi incluído no projeto — adicione o seu próprio arquivo nesse caminho caso queira o player funcional.
- **Vídeo**: o `<iframe>` aponta para um identificador de vídeo do YouTube incluído apenas como exemplo de incorporação responsiva — substitua pelo vídeo desejado.

---

Bons estudos! 🌅☕
