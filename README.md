# Conecta Bairro — Página Acessível

Atividade prática de **Acessibilidade Web e HTML Semântico**.

Página de um projeto social fictício de inclusão digital, desenvolvida apenas com
**HTML5 e CSS3**, sem frameworks, bibliotecas ou JavaScript.

## Como visualizar

Baixe o repositório e abra o arquivo `index.html` em qualquer navegador.
Não há dependências, servidor ou etapa de compilação.

## Estrutura dos arquivos

```
pagina-inclusiva/
├── index.html                        página principal
├── css/
│   └── estilo.css                    toda a apresentação visual
├── img/
│   ├── logo.svg                      logotipo do projeto
│   ├── favicon.svg                   ícone da aba do navegador
│   └── oficina.svg                   ilustração da turma da oficina
├── docs/
│   ├── tutorial-acessibilidade.pdf   TUTORIAL COMPLETO (documento de entrega)
│   ├── tutorial.html                 fonte do tutorial
│   └── captura-*.png                 capturas de tela do projeto
└── README.md
```

## Requisitos de estrutura atendidos

| Requisito | Onde está |
|---|---|
| Cabeçalho | `<header>` com logotipo, `<h1>` e slogan |
| Menu de navegação | `<nav aria-label="Menu principal">` com 4 links |
| Conteúdo principal | `<main id="conteudo">` |
| Pelo menos 3 seções | 4 `<section>`: sobre, oficinas, depoimentos e inscrição |
| Imagem com texto alternativo | `<figure>` + `<img alt="...">` + `<figcaption>` |
| Lista de informações | 8 listas (`<ul>` / `<li>`), 25 itens |
| Formulário acessível | 4 `<fieldset>` + `<legend>`, 11 campos rotulados |
| Links e botões | links descritivos e 2 `<button>` nativos |
| Rodapé | `<footer>` com contato, horários e links úteis |

## Recursos de acessibilidade implementados

- **Idioma declarado** — `<html lang="pt-BR">` (WCAG 3.1.1)
- **Hierarquia de títulos** — um único `h1`, sem saltos de nível (WCAG 1.3.1)
- **HTML semântico** — `header`, `nav`, `main`, `section`, `article`, `aside`,
  `figure`, `figcaption`, `form`, `fieldset`, `legend`, `button`, `footer`
- **Imagens com `alt`** descritivo (WCAG 1.1.1)
- **`<label for>` associado a todos os campos**, mais `aria-describedby` nos
  textos de ajuda (WCAG 1.3.1 e 3.3.2)
- **Links e botões com texto descritivo** — nada de "clique aqui" (WCAG 2.4.4)
- **Contraste conferido** — todos os pares medidos, mínimo obtido de 4,63:1
  (WCAG 1.4.3 e 1.4.11)
- **Navegação apenas por teclado** — 23 paradas de `Tab`, na ordem do conteúdo
- **Foco sempre visível** — anel de 3 px em `:focus` / `:focus-visible`, com cor
  ajustada em fundos escuros (WCAG 2.4.7)
- **Link de salto** para o conteúdo principal (WCAG 2.4.1)
- **Alvos de toque de 48 px** nos botões (WCAG 2.5.8)
- **Layout responsivo** sem rolagem horizontal (WCAG 1.4.10)
- **`prefers-reduced-motion`** e **`forced-colors`** respeitados

## Tutorial

O tutorial completo, com os trechos de código comentados, as capturas de tela e
os resultados dos testes de acessibilidade, está em
[`docs/tutorial-acessibilidade.pdf`](docs/tutorial-acessibilidade.pdf).
