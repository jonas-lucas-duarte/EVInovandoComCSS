# Módulo 2 - Exemplo de Criação

### Sintaxe do CSS

A regra do CSS é dividida em duas partes principais: o **seletor** e uma (ou mais) **declarações**.

```h1 {color: blue; font-size: 12px}```

- `h1`: O seletor é o elemento HTML que receberá a formatação.

- `color:` e `font-size:`: A propriedade é o atributo do estilo que será alterado.

- `blue` e `12px`: Cada propriedade tem um valor.

### Inserindo o CSS no Código HTML

```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.0//EN">

<html>
<head>
<style type="text/css">
	h1 {color: red}
	p {color: grey}
</style>
</head>
<body>
<h1>Exemplo de Cabeçalho</h1>
<p>Exemplo de Parágrafo</p>
</body>
</html>
```

### Inserindo o CSS por meio de um Arquivo Externo

Para inserir o CSS por meio de um arquivo externo é preciso ter dois arquivos: uma página HTML (.html) e uma folha de estilos (.css).

O CSS é identificado pela declaração:

`/* CSS Document */`

#### Exemplo 1

```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.0//EN">

<html>
<head>
<link rel="stylesheet" type="text/css" href="codigo1.css">
</head>
<body>
<h1>Este H1 terá a fonte no tamanho 20</h1>
<h2>Este H2 terá a cor vermelha</h2>
<p>Este parágrafo terá a margem esquerda de 50 pixels</p>
</body>
</html>
```

```css
/* CSS Document */

body {
	background-color: pink;
}

h1 {
	font-size: 20px;
}

h2 {
	color: red;
}

p {
	margin-left: 50px;
}
```

#### Exemplo 2

```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.0//EN">

<html>
<head>
<link rel="stylesheet" type="text/css" href="codigo2.css">
</head>
<body>
<h1>Este H1 terá a fonte na cor marrom</h1>
<p>Este parágrafo mostra que o estilo do texto foi formatado com a fonte 16, e tem uma margem de 20 pixels</p>
<p><a href="http:www.ev.org.br" target="_blank">Este link também tem um estilo personalizado pelo CSS</a></p>
</body>
</html>
```

```css
/* CSS Document */

body {
	background-color: tan;
}

h1 {
	color: marron;
}

h2 {
	color: navy;
}

p {
	font-size: 16px;
	margin-left: 20px;
}

a:link {color: green}

a:visited {color: yellow}

a:hover {color: black}

a:active {color: blue}
```

### Escrevendo o Código CSS

As declarações terminarão com **ponto e vírgula** (;) e os grupos de declarações são cercados por **chaves** ({}).

`p {color: red; text-align: center;}`

Para que o código fique mais legível.

```css
p {
	color: red;
	text-align: center;
}
```

`p {background-color: red;}`

- `p`: O primeiro passo é selecionar o elemento que receberá o estilo, nesse caso o \<p\>. Observer que em CSS, não se coloca o \<\> em volta do nome.

- `{...}`: Coloque todos os estilos do elemento \<p\> entre chaves.

- `background-color`: Especifica a propriedade que o estilo terá, nesse caso a cor de fundo do elemento \<p\>.

- `:`: Há dois pontos entre a propriedade e seu valor.

- `red`: Defina a cor de fundo como vermelho.

- `;`: No final, coloque um ponto-e-vírgula.

- `p {background-color: red;}`: Chamamos tudo isso de REGRA.

### Quer Adicionar mais Estilos?

```css
p {
	background-color: rede;
	border: 1px solid gray;
}
```

> Colocar uma borda em torno de seu parágrafo.

### Comentários

`/*Seu comentário*/`

> Quanto mais detalhes melhor.

```css
/* CSS Document */

/*Propriedades para formatação do texto.
O texto será alinhado a direita com cor azul e fonte Arial*/

p {
	text-align: right;
	color: blue;
	font-family: arial;
}
```