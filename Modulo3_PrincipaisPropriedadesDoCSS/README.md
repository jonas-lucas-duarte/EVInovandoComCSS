# Módulo 3 - Principais Propriedades do CSS

### Cores

As cores na *web* são representadas por um sistema de cores aditivas, chamado **RGB**, sigla das cores *Red*, *Green* e *Blue*.

RGB é um sistema **hexaxecimal (base 16)**: vai do 0 ao 9 e, em seguida, do A ao F (o "A" seria o 10, o "B" o 11 e assim sucessivamente).

### Propriedade Color

```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.0//EN">

<html>
<head>
<style type="text/css">
	p {color: #89A010}
</style>
</head>
<body>
<p>Exemplo de Parágrafo</p>
</body>
</html>
```

Nesse exemplo, a propriedade ***color*** define a cor do texto do parágrafo `<p></p>`.

### Background-color

Define a cor do plano de fundo nos elementos de uma página.

```
/* CSS Document */

body {
	background-color: #90CDE6;
}
```

> Quando trabalhamos com CSS as cores podem ser definidas por três formas diferentes.
>
> - Valores hexadecimais: "#FF0000";
> - Valores RGB: "rgb(255,0,0)";
> - Nome da cor: "red";

### Background-image

Define uma imagem como plano de fundo.

```css
/* CSS Document */

body {
	background-image: url('imagem.gif')
}
```

### Background-repeat

Estabelece uma forma específica de repetição.

#### HORIZONTAL

```css
/* CSS Document */

body {
	background-image: url('imagem.gif');
	background-repeat: repeat-x;
}
```

#### VERTICAL

```css
/* CSS Document */

body {
	background-image: url('imagem.gif');
	background-repeat: repeat-y;
}
```

#### NO-REPEAT

```css
/* CSS Document */

body {
	background-image: url('imagem.gif');
	background-repeat: no-repeat;
}
```

### Background-attachment

Pode-se definir que o plano de fundo inserido será fixo ou se ele rolará com o restante da página.

#### Fixed

```css
/* CSS Document */

body {
	background-image: url('imagem.gif');
	background-repeat: no-repeat;
	background-attachment: fixed;
}
```

O plano de fundo será fixo.

#### Scroll

```css
/* CSS Document */

body {
	background-image: url('imagem.gif');
	background-repeat: no-repeat;
	background-attachment: scroll;
}
```

O plano de fundo rolará com o restante da página (padrão).

### Background-position

Especificar o posicionamento da imagem de fundo.

```css
/* CSS Document */

body {
	background-image: url('imagem.gif');
	background-repeat: no-repeat;
	background-positon: right top;
}
```

- x-posição y-posição
- x-porcentagem y-porcentagem
- top left
- top center
- top right
- center left
- center center
- center right
- bottom left
- bottom center
- bottom right