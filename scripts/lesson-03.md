# Lección 03 — HTML: listas, imágenes y enlaces

**Duración estimada:** 8 minutos  
**Tema:** Listas, imágenes y enlaces en HTML  
**Herramienta de práctica:** JSFiddle  
**Conocimientos previos:** Estructura básica de HTML, títulos y párrafos.

# Objetivos de aprendizaje

Al finalizar esta lección, el estudiante podrá:

- Identificar los dos tipos principales de listas en HTML.
- Crear listas desordenadas con `ul` y `li`.
- Crear listas ordenadas con `ol` y `li`.
- Insertar imágenes con la etiqueta `img` y los atributos `src`, `alt` y `width`.
- Crear enlaces con la etiqueta `a` y los atributos `href` y `target`.
- Organizar la información de una página web mediante listas.
- Combinar listas, imágenes y enlaces en una misma página.

# 0:00 – 0:32 | Introducción

¡Hola a todos!

Bienvenidos a la lección número 3.

En las lecciones anteriores aprendimos qué es el desarrollo web y conocimos los dos componentes fundamentales de una página: HTML y CSS.

Después, en nuestra segunda lección, aprendimos a crear nuestra primera página HTML utilizando su estructura básica, títulos y párrafos.

Hoy vamos a incorporar tres elementos muy importantes: listas, imágenes y enlaces.

Partimos de la página sobre Machu Picchu que ya tenemos en nuestro editor.

Nuestra página ya tiene un encabezado (`header`), un contenido principal (`main`) y varias secciones (`section`) con títulos y párrafos.

Vamos a agregarlos uno por uno.

```text
HTML = Estructura y contenido

Listas + Imágenes + Enlaces = Página más completa
```

# 0:32 – 1:52 | Listas desordenadas

Primero vamos a aprender a crear listas en HTML.

Existen dos tipos principales de listas: las listas desordenadas y las listas ordenadas.

Para crear una lista desordenada utilizamos la etiqueta `ul`, que muestra los elementos con viñetas.

`ul` viene de unordered list, que significa lista desordenada.

Dentro de ella utilizamos la etiqueta `li` para escribir cada elemento de la lista.

`li` viene de list item, que significa elemento de lista.

En nuestra página vamos a colocar algunas actividades que podemos realizar en Machu Picchu.

Dentro de la sección "¿Qué puedes hacer?", después del título "Actividades principales", agregamos lo siguiente:

```html
<h3>Actividades principales</h3>
<ul>
  <li>Visitar las ruinas incaica</li>
  <li>Tomar fotografias del paisaje</li>
  <li>Conocer la historia de los incas</li>
  <li>Disfrutar de la naturaleza</li>
</ul>
```

Cada `li` representa un elemento de la lista.

Al escribir el código, el navegador muestra automáticamente una viñeta delante de cada actividad.

No necesitamos escribir las viñetas manualmente.

```text
ul → Lista desordenada
li → Cada elemento de la lista
```

Las listas nos permiten organizar mejor la información de nuestra página.

# 1:52 – 2:54 | Listas ordenadas

Ahora también vamos a crear una lista ordenada utilizando la etiqueta `ol`.

`ol` viene de ordered list, que significa lista ordenada.

A diferencia de la lista anterior, esta lista muestra números automáticamente.

Podemos utilizarla para explicar los pasos necesarios para visitar Machu Picchu.

Agregamos un nuevo título y la lista ordenada:

```html
<h3>Los 3 pasos para visitarlo</h3>
<ol>
  <li>Viajar a Cuzco</li>
  <li>Comprar las entradas</li>
  <li>Realizar el recorrido turistico</li>
</ol>
```

En este caso, el orden de los elementos sí importa.

Primero viajamos a Cuzco, después compramos las entradas y finalmente realizamos el recorrido turístico.

El navegador numera cada paso de forma automática.

```text
ul → Lista con viñetas

ol → Lista con números

li → Cada elemento de la lista
```

# 2:54 – 3:15 | Organizando la información

Como podemos observar, las listas nos permiten organizar mejor la información de nuestra página.

Ahora la sección "¿Qué puedes hacer?" tiene dos partes bien diferenciadas: las actividades principales y los pasos para visitar Machu Picchu.

A continuación vamos a incorporar un elemento visual.

# 3:15 – 5:12 | Imágenes

Ahora vamos a agregar una imagen a nuestra página web.

Para hacerlo utilizamos la etiqueta `img`.

Esta etiqueta tiene un atributo llamado `src`, donde colocamos la dirección de la imagen que queremos mostrar.

También utilizamos el atributo `alt`, que sirve para describir la imagen en caso de que no pueda cargarse y facilita la accesibilidad.

`alt` viene de alternative text, que significa texto alternativo.

Además, podemos utilizar el atributo `width` para establecer el ancho de la imagen.

En nuestro ejemplo utilizaremos un ancho de 500 píxeles.

Vamos a colocar una fotografía de Machu Picchu utilizando una dirección de Internet.

```html
<img
  src="https://images.unsplash.com/photo-1526392060635-9d6019884377?w=900"
  alt="Vista panorámica de Machu Picchu"
  width="500"
>
```

La etiqueta `img` no tiene etiqueta de cierre.

Los atributos se escriben dentro de la etiqueta de apertura.

```text
img   → Imagen

src   → Dirección de la imagen

alt   → Descripción de la imagen

width → Ancho de la imagen
```

Al aplicar el cambio, la imagen aparece en nuestra página y el contenido resulta mucho más atractivo.

# 5:12 – 6:38 | Enlaces

El siguiente elemento que vamos a aprender son los enlaces.

Para crear un enlace utilizamos la etiqueta `a`.

Esta etiqueta utiliza el atributo `href`, donde colocamos la dirección de la página a la que queremos dirigir al usuario.

El texto que escribimos entre `<a>` y `</a>` es el que el usuario puede pulsar para visitar la página.

En nuestro ejemplo vamos a agregar un enlace hacia la página oficial de Machu Picchu, dentro de la sección "Más información".

```html
<a href="https://www.machupicchu.gob.pe/"
   target="_blank">Conoce más sobre Machu Picchu</a>
```

También utilizamos el atributo `target="_blank"`, que permite abrir el enlace en una nueva pestaña del navegador.

De esta manera, el usuario podrá obtener más información sin perder nuestra página principal.

```text
a      → Enlace

href   → Dirección de destino

target → Dónde se abre el enlace
```

Los enlaces son muy importantes porque permiten conectar diferentes páginas y facilitar la navegación.

# 6:38 – 7:32 | Repaso rápido

Hagamos un pequeño repaso.

Aprendimos a utilizar tres elementos fundamentales de HTML.

Primero, las listas ordenadas y desordenadas para organizar información.

Segundo, las imágenes mediante la etiqueta `img` para agregar contenido visual.

Y tercero, los enlaces mediante la etiqueta `a` para conectar nuestra página con otros sitios web.

```html
<ul>
  <li>Elemento con viñeta</li>
</ul>

<ol>
  <li>Elemento numerado</li>
</ol>

<img src="imagen.jpg" alt="Descripción" width="500">

<a href="https://ejemplo.com">Texto del enlace</a>
```

Con estos elementos podemos crear páginas mucho más completas e interesantes.

Nuestra página sobre Machu Picchu ya tiene títulos, párrafos, listas, una imagen y un enlace.

# 7:52 – 8:02 | Cierre

¡Excelente trabajo!

Ahora sabes crear listas, imágenes y enlaces en HTML.

Con estos tres elementos nuestra página sobre Machu Picchu es mucho más completa.

En la siguiente lección aprenderemos CSS para cambiar su apariencia: colores, fuentes, bordes y mucho más.

Y recuerda: la mejor manera de aprender es practicar y experimentar con el código.

Nos vemos en la siguiente lección.


## Tu reto HTML

- Agrega una actividad más a la lista

- Cambia la imagen y su ancho

- Agrega otro enlace

- Observa el resultado

- Experimenta
