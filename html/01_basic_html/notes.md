# Basic HTML Review

## O que é HTML

* HTML = **HyperText Markup Language**
* Usado para estruturar conteúdo na web: textos, imagens, links, seções, listas, etc.

---

## Elementos básicos (tags)

| Tag                 | Uso / Descrição                                                |
| ------------------- | -------------------------------------------------------------- |
| `<!DOCTYPE html>`   | Declaração do tipo de documento (HTML5).                       |
| `<html>`            | Raiz do documento HTML.                                        |
| `<head>`            | Cabeçalho: contém metadados, título, ligação a estilos etc.    |
| `<title>`           | Define título da página (aparece na aba do navegador).         |
| `<body>`            | Corpo da página, onde fica o conteúdo visível.                 |
| `<h1>` … `<h6>`     | Cabeçalhos de diferentes níveis; `<h1>` o mais importante.     |
| `<p>`               | Parágrafo.                                                     |
| `<a>`               | Link (âncora). Atributo principal: `href`.                     |
| `<img>`             | Imagem. Principais atributos: `src`, `alt`.                    |
| `<ul>` / `<ol>`     | Listas: `<ul>` lista não ordenada, `<ol>` lista ordenada.      |
| `<li>`              | Item de lista (usado dentro de `<ul>` ou `<ol>`).              |
| `<div>`             | Divisão, contêiner genérico.                                   |
| `<span>`            | Inline, contêiner genérico.                                    |
| `<br>`              | Quebra de linha.                                               |
| `<hr>`              | Linha horizontal (separador).                                  |
| `<em>` / `<strong>` | `<em>` enfatiza (itálico), `<strong>` = importância (negrito). |

---

## Atributos importantes

* `href` para links (`<a href="url">`)
* `src` e `alt` para imagens
* `target` para links, ex: `target="_blank"` abre em nova aba
* `id` e `class` para identificar ou agrupar elementos
* `title` para fornecer informação extra ao passar o mouse (tooltip)

---

## Hierarquia / Aninhamento

* Elementos HTML formam uma árvore.
* Algumas regras:

  * `<html>` contém `<head>` e `<body>`.
  * Tags de bloco vs tags inline.
  * Deve-se fechar tags onde for necessário (ex: `<p>`, `<div>`), embora algumas tags sejam auto-fechadas (`<img />`, `<br />`).

---

## Texto e formatações

* Quebras, espaços múltiplos: HTML ignora múltiplos espaços — usar tags ou CSS para controle visual.
* Tags de texto:

  * `<strong>` e `<b>` — negrito
  * `<em>` e `<i>` — itálico / ênfase
  * `<small>`, `<mark>`, `<del>`, `<ins>` etc (dependendo do escopo estudado)
* Citações:

  * `<blockquote>` para citações longas
  * `<q>` para citações curtas inline

---

## Links e navegação

* `<a href="…">texto</a>` básico
* Atributos como `target="_blank"` para abrir nova aba
* Pode linkar para:

  * outras páginas externas
  * páginas internas (relativas)
  * âncoras dentro da mesma página (`id` + `href="#id"`)

---

## Imagens

* `<img src="caminho" alt="texto descritivo">`
* `alt` importante por acessibilidade e SEO
* Pode adicionar atributos como `width`, `height` (embora controle de tamanho via CSS seja preferível)

---

## Estrutura básica de uma página HTML5

```html
<!DOCTYPE html>
<html lang="pt">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Título da Página</title>
  </head>
  <body>

    <h1>Meu título principal</h1>
    <p>Um parágrafo de exemplo.</p>
    <a href="https://exemplo.com" target="_blank">Link para o exemplo</a>
    <img src="imagem.jpg" alt="Descrição da imagem">

    <ul>
      <li>Item 1</li>
      <li>Item 2</li>
    </ul>

  </body>
</html>
```

---

## Boas práticas

* Sempre usar `alt` em imagens
* Estruturar bem: títulos, seções, listas em vez de tudo num só parágrafo
* Usar nomes de classes / ids significativos
* Evitar inline styles quando possível (usar CSS externo)
* Garantir acessibilidade básica (semântica, tags apropriadas)

---
