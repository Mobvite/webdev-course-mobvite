# Lección 04 — Introducción a CSS

**Duración estimada:** 12 minutos  
**Tema:** Introducción a CSS  
**Herramienta de práctica:** JSFiddle  
**Conocimientos previos:** HTML básico, encabezados, párrafos, listas, imágenes y enlaces.

# Objetivos de aprendizaje

Al finalizar esta lección, el estudiante podrá:

- Explicar para qué sirve CSS.
- Identificar un selector, una propiedad y un valor.
- Cambiar colores de texto y de fondo.
- Modificar fuentes y tamaños de texto.
- Añadir bordes y espacios.
- Centrar texto mediante CSS.
- Personalizar visualmente una página web sencilla.

# 0:00 – 0:40 | Introducción

En la lección anterior construimos una página web sobre Machu Picchu utilizando HTML.

Agregamos títulos, párrafos, una imagen, listas y un enlace.

Nuestra página ya tiene contenido y una estructura, pero todavía se ve bastante sencilla.

En esta lección vamos a cambiar eso.

Aprenderemos a utilizar CSS para agregar colores, cambiar fuentes, crear bordes y mejorar la apariencia de nuestra página.

Al terminar, nuestra página sobre Machu Picchu tendrá una apariencia mucho más atractiva.

```text
HTML = Estructura
CSS = Apariencia
```

```text
ANTES                 DESPUÉS
Solo HTML         →   HTML + CSS
```

# 0:40 – 1:50 | ¿Qué es CSS?

CSS significa Hojas de Estilo en Cascada.

Pero no necesitas memorizar ese nombre por ahora.

Lo importante es entender una idea muy sencilla.

HTML le indica al navegador qué elementos existen en nuestra página.

CSS le indica al navegador cómo queremos que se vean esos elementos.

Podemos imaginar que estamos construyendo una casa.

HTML serían las paredes, las puertas y las habitaciones.

CSS sería la pintura, los colores y la decoración.

En nuestro caso, HTML ya nos permitió agregar toda la información sobre Machu Picchu.

Ahora CSS nos permitirá decidir cómo queremos presentar esa información.

```text
HTML
Define la estructura

CSS
Define la apariencia
```

```text
HTML + CSS = Página web
```

# 1:50 – 2:20 | Conociendo JSFiddle

Para practicar utilizaremos JSFiddle.

JSFiddle es un editor que funciona directamente desde nuestro navegador.

No necesitamos instalar ningún programa.

En nuestra pantalla podemos encontrar diferentes áreas para escribir HTML y CSS, además de una sección donde veremos el resultado de nuestra página.

En el área HTML ya tenemos el código de la página sobre Machu Picchu que desarrollamos anteriormente.

Durante esta lección trabajaremos principalmente en el área de CSS.

```text
HTML   → Estructura
CSS    → Estilos
Result → Resultado
```

# 2:20 – 3:35 | Nuestra primera regla CSS

Comencemos cambiando el color del título principal de nuestra página.

En el área de CSS vamos a escribir nuestra primera regla.

```css
h1 {
  color: royalblue;
}
```

Una regla de CSS tiene varias partes importantes.

Primero tenemos `h1`.

Esto se llama selector.

El selector indica qué elemento de HTML queremos modificar.

En este caso queremos modificar el título principal: "Mi lugar turístico favorito".

Luego tenemos `color`.

Esto se llama propiedad.

La propiedad indica qué característica queremos cambiar.

Finalmente tenemos `royalblue`.

Este es el valor.

El valor indica cómo queremos modificar esa propiedad.

```text
h1        → Selector

color     → Propiedad

royalblue → Valor
```

Cuando aplicamos la regla, podemos observar inmediatamente que nuestro título cambia de color.

# 3:35 – 4:45 | Cambiando el fondo

Ahora cambiemos el fondo de toda nuestra página.

Para modificar el fondo general utilizaremos el selector `body`.

Agregaremos la propiedad `background-color`.

```css
body {
  background-color: #f4f4f4;
}
```

La propiedad `background-color` nos permite cambiar el color de fondo.

En este ejemplo utilizamos un código de color hexadecimal.

Estos códigos comienzan con el símbolo numeral seguido de diferentes números o letras.

No necesitas memorizar estos códigos.

También podemos utilizar nombres sencillos de colores.

Por ejemplo, probemos con `lightblue`.

```css
body {
  background-color: lightblue;
}
```

Podemos observar inmediatamente cómo cambia el aspecto de nuestra página.

Ahora volvamos a utilizar un tono más claro.

```css
body {
  background-color: #f4f4f4;
}
```

Puedes experimentar con diferentes colores hasta encontrar uno que te guste.

CSS nos permite comenzar a darle personalidad a nuestra página.

# 4:45 – 6:05 | Fuentes y tamaño del texto

También podemos utilizar CSS para cambiar la apariencia del texto.

Vamos a modificar la fuente de toda nuestra página.

Actualizamos la regla de `body`:

```css
body {
  background-color: #f4f4f4;
  font-family: Arial, sans-serif;
}
```

La propiedad `font-family` indica qué tipo de fuente queremos utilizar.

En este ejemplo utilizamos Arial.

También colocamos `sans-serif` como una segunda opción en caso de que la primera fuente no se encuentre disponible.

Ahora vamos a aumentar ligeramente el tamaño de nuestros párrafos.

```css
p {
  font-size: 18px;
}
```

La propiedad `font-size` controla el tamaño del texto.

En este caso utilizamos un tamaño de dieciocho píxeles.

Podemos observar que las descripciones sobre Machu Picchu ahora son un poco más grandes y fáciles de leer.

```text
font-family → Tipo de fuente
font-size   → Tamaño del texto
```

# 6:05 – 7:10 | Aplicando estilos a otros elementos

Podemos utilizar diferentes selectores para cambiar distintas partes de nuestra página.

Por ejemplo, nuestra página contiene varios títulos secundarios creados con `h2`.

Podemos darles otro color.

```css
h2 {
  color: darkblue;
}
```

Ahora los títulos como "Conoce Machu Picchu", "¿Qué puedes hacer?" y "Más información" utilizan este nuevo color.

Nuestro título principal sigue utilizando el color que configuramos anteriormente.

Esta es una de las ideas más importantes de CSS.

Los selectores nos permiten elegir qué elementos queremos modificar.

# 7:10 – 8:50 | Bordes y espacios

Nuestra página también contiene listas con actividades y pasos para visitar Machu Picchu.

Vamos a hacer que estas listas destaquen un poco más utilizando un fondo, un borde y espacio interior.

Primero podemos aplicar el estilo a nuestra lista de actividades.

```css
ul {
  background-color: white;
  border: 2px solid royalblue;
  padding: 20px;
}
```

Analicemos estas propiedades.

`background-color` coloca un fondo blanco en nuestra lista.

`border` crea una línea alrededor del elemento.

En este caso indicamos que el borde debe tener dos píxeles de grosor, utilizar una línea sólida y ser de color azul.

Finalmente tenemos `padding`.

Esta propiedad crea espacio entre el contenido y el borde del elemento.

```text
border  → Borde alrededor del elemento

padding → Espacio dentro del elemento
```

Si eliminamos temporalmente:

```css
padding: 20px;
```

podemos observar que el texto queda mucho más cerca del borde.

Al volver a agregarlo, la lista resulta más fácil de leer.

Podemos utilizar este mismo estilo en otras listas de nuestra página más adelante.

# 8:50 – 9:50 | Centrando el título

Hagamos un último cambio visual.

Vamos a centrar nuestro título principal.

Para hacerlo utilizaremos la propiedad `text-align`.

Actualizamos nuestra regla:

```css
h1 {
  color: royalblue;
  text-align: center;
}
```

El valor `center` indica que queremos colocar el texto en el centro.

Nuestro título "Mi lugar turístico favorito" ahora destaca mucho más en la parte superior.

Y lo más importante es que no tuvimos que modificar nuestro HTML.

Solamente modificamos su apariencia mediante CSS.

```text
HTML → Qué contiene la página

CSS → Cómo se ve la página
```

# 9:50 – 10:50 | Repaso rápido

Hagamos un pequeño repaso.

Una regla CSS comienza con un selector.

El selector indica qué elemento queremos modificar.

Dentro de las llaves escribimos diferentes declaraciones.

Cada declaración utiliza una propiedad y un valor.

Durante esta lección utilizamos CSS para modificar colores, fondos, fuentes, tamaño del texto, bordes, espacios y alineación.

```css
h1 {
  color: royalblue;
  text-align: center;
}
```

```text
h1        → Selector

color     → Propiedad

royalblue → Valor
```

Nuestra página sigue teniendo exactamente el mismo contenido HTML sobre Machu Picchu.

Lo único que hemos cambiado es su apariencia.

# 10:50 – 11:40 | Reto práctico

Ahora es tu turno.

Antes de terminar la lección, quiero proponerte un pequeño reto.

Personaliza la página de Machu Picchu para que tenga tu propio estilo.

Intenta cambiar por lo menos tres cosas.

Puedes cambiar el color del fondo.

Puedes cambiar el color del título principal.

Puedes probar otra fuente.

También puedes cambiar el color o el grosor del borde de la lista de actividades.

No existe un único diseño correcto.

El objetivo es experimentar y observar cómo cada propiedad modifica nuestra página.

Pausa el video y prueba tus propios estilos en JSFiddle.

### Tu reto CSS

```text
✓ Cambia el color de fondo

✓ Cambia el color del título

✓ Prueba otra fuente

✓ Modifica el borde de la lista

✓ Experimenta
```

# 11:40 – 12:00 | Cierre

¡Excelente trabajo!

Ahora conoces los conceptos básicos de CSS y sabes cómo utilizarlo junto con HTML.

Comenzamos con la página de Machu Picchu que construimos en la lección anterior y conseguimos mejorar su apariencia sin cambiar su contenido.

HTML nos permite construir la estructura de una página.

CSS nos permite controlar su apariencia.

En la siguiente lección continuaremos combinando ambos para construir una página cada vez más completa.

Y recuerda: no tienes que memorizar todas las propiedades de CSS.

La mejor manera de aprender es experimentar, cambiar valores y observar qué ocurre.

Nos vemos en la siguiente lección.
