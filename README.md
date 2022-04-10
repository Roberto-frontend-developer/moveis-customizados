# moveis-customizados

Fala Dev! 💜

Objetvo dessa projeto é desenvolver  tags html semânticas.


## tags html semântico
```
<header> é utilizado para representar o cabeçalho de um documento ou seção declarado no HTML. Nele podemos inserir elementos de <h1> a <h6>

<section> representa uma seção dentro de um documento e geralmente contém um título, o qual é definido por meio de um dos elementos entre <h1> e <h6>

<article> quando precisamos declarar um conteúdo que não precisa de outro para fazer sentido em um documento HTML

<nav> é utilizado quando precisamos representar um agrupamento de links de navegação, que, por sua vez, são criados com os elementos <ul>, <li> e <a>.

<aside> é utilizado quando precisamos criar um conteúdo de apoio/adicional ao conteúdo principal.

<main> especifica o conteúdo principal e, consequentemente, de maior relevância dentro da página. 

<figure> é uma marcação de uso específico para a inserção de uma figura.

<footer> representa um rodapé de um documento, como a área presente no final de uma página web

<a> é descrever um link, conectando os diversos documentos de um site e permitindo a navegação por esse conteúdo.

<em> é utilizado quando desejamos enfatizar um trecho ou palavra no texto, indicando que ela contribui de forma mais relevante para o sentido/compreensão do conteúdo.

<strong> também é utilizado para destacar uma parte do texto.

<cite> é utilizado para declarar que naquele trecho há uma citação, isto é, um trecho de texto que não foi escrito pelo autor do conteúdo.

<q> responsável por apresentar o conteúdo retirado de outra fonte.

<time> é utilizado para representar datas
```
## CSS Units

Unidades de medidas do CSS

Layout Fixo
`px` - Pixels

Layout Fluido
`%` - Porcentagem
`auto` - Automática
`vh` - Viewport Height
`vw` - Viewport Width

Textos fixos
`1px` = 0.75pt
`16px` = 12pt

Texto fluidos
`em` - multiplicado pelo pai 
`rem` - multiplicado pelo root

## CSS Media Queries 

No HTMl eu coloco a seguinte tag meta

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

No CSS eu uso da seguinte forma

```css
@media (max-width: 320px) {
  #form h3 {
    font-size: 2rem;
  }
}
```

## HTML Media Attrib.

Posso utilizar o atribuito `media` no link do meu HTML, ao importar um arquivo css, usando as propriedades da mesma forma que usaria na regra `@media` do css.

```html
<link 
    rel="stylesheet"
    href="responsive.css" 
    media="screen and (max-width: 768px)"
/>

<link rel="stylesheet" href="print.css" media="print">
```

## Imagens

Usamos a tag `<picture>` para que as imagens sejam responsivas.

```html
<picture class="image" alt="Imagem">
    <source media="(min-width: 768px)" 
        srcset="https://i.ytimg.com/vi/GykTLqODQuU/maxresdefault.jpg">
    <source media="(min-width: 320px)" 
        srcset="https://i.ytimg.com/vi/GykTLqODQuU/hqdefault.jpg">
    <source media="(min-width: 10px)" 
        srcset="https://i.ytimg.com/vi/GykTLqODQuU/mqdefault.jpg">

    <img 
        src="https://i.ytimg.com/vi/GykTLqODQuU/hqdefault.jpg" 
        alt="Imagem" />
</picture>
```

Sempre que possível, usar SVG ao invés de JPG, PNG
