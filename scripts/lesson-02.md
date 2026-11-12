# Lección 02 — Introducción a HTML

**Duración estimada:** 10 minutos  
**Tema:** Introducción a HTML  
**Herramienta de práctica:** CodePen  
**Conocimientos previos:** Ninguno. Solo haber visto la lección 1.

# Objetivos de aprendizaje

Al finalizar esta lección, el estudiante podrá:

- Explicar para qué sirve HTML.
- Reconocer una etiqueta de apertura y una de cierre.
- Escribir un título y un párrafo.
- Identificar las partes básicas de una página HTML.
- Comprender qué es un atributo.
- Crear su primera página web en un editor en línea.

# 0:00 – 0:40 | Introducción

En la lección anterior descubrimos que una página web está hecha de contenido y de estilo.

El contenido se escribe con HTML.

El estilo se escribe con CSS.

En esta lección vamos a comenzar por el contenido.

Vamos a crear nuestra primera página web sobre un lugar turístico del Perú: Machu Picchu.

No necesitas instalar ningún programa.

Solo necesitas un navegador.

```text
Sitio web = HTML (contenido) + CSS (estilo)

Hoy: HTML
```

# 0:40 – 1:50 | ¿Qué es HTML?

HTML significa Lenguaje de Marcado de Hipertexto.

No necesitas memorizar ese nombre.

Lo importante es esta idea.

HTML sirve para decirle al navegador qué es cada parte del contenido.

Por ejemplo: esto es un título, esto es un párrafo, esto es una lista.

Podemos imaginar un cuaderno con separadores de colores.

Cada separador indica qué tipo de información hay en esa parte.

En HTML, esos separadores se llaman etiquetas.

```text
HTML = Le dice al navegador
       qué es cada parte del contenido
```

# 1:50 – 2:30 | Conociendo CodePen

Para practicar utilizaremos CodePen.

CodePen es un editor que funciona directamente en el navegador.

No necesitas crear una cuenta para empezar a escribir.

Veremos tres áreas: HTML, CSS y JS.

Hoy solo utilizaremos el área HTML.

Debajo, o al costado según el tamaño de la pantalla, aparece el resultado de lo que escribimos.

El enlace a este editor está en la descripción del video.

```text
HTML   → Aquí escribimos
CSS    → Hoy no lo usamos
JS     → Hoy no lo usamos
Result → Aquí vemos la página
```

# 2:30 – 4:00 | Etiquetas y elementos

Una etiqueta se escribe entre los símbolos "menor que" y "mayor que".

Casi todos los elementos tienen dos etiquetas: una de apertura y una de cierre.

La etiqueta de cierre lleva una barra inclinada.

Escribamos un título.

```html
<h1>Mi lugar turístico favorito</h1>
```

Aquí `<h1>` es la etiqueta de apertura.

`</h1>` es la etiqueta de cierre.

Lo que está en medio es el contenido.

Todo junto, desde la apertura hasta el cierre, se llama elemento.

Al escribirlo, el resultado muestra un título grande en la parte superior.

```text
<h1>  Texto  </h1>
 ↑      ↑      ↑
Abre  Contenido  Cierra

Etiqueta + contenido + etiqueta = Elemento
```

# 4:00 – 5:00 | Nuestro primer párrafo

Ahora agreguemos un texto debajo del título.

Para escribir un párrafo utilizamos la etiqueta `<p>`.

```html
<h1>Mi lugar turístico favorito</h1>
<p>Conoce uno de los lugares más bonitos del Perú.</p>
```

Cada párrafo nuevo lleva sus propias etiquetas de apertura y de cierre.

Si olvidamos la etiqueta de cierre, el navegador puede mostrar la página de forma incorrecta.

Por eso, una buena costumbre es escribir las dos etiquetas desde el inicio y luego colocar el contenido en medio.

```text
<h1> → Título principal

<p>  → Párrafo
```

# 5:00 – 6:30 | La estructura de una página HTML

Hasta ahora escribimos solo dos elementos.

Pero una página HTML completa tiene una estructura básica.

Veamos cómo es.

```html
<!doctype html>
<html lang="es">
  <head>
    <title>Mi lugar favorito</title>
  </head>
  <body>
    <h1>Mi lugar turístico favorito</h1>
    <p>Conoce uno de los lugares más bonitos del Perú.</p>
  </body>
</html>
```

La primera línea indica al navegador que el documento es una página HTML.

El elemento `html` contiene toda la página.

Dentro tenemos dos partes.

La primera es `head`, que significa cabeza.

Aquí va información sobre la página que no se muestra en pantalla, como el título que aparece en la pestaña del navegador.

La segunda es `body`, que significa cuerpo.

Aquí va todo lo que la persona ve en la página: títulos, párrafos, imágenes y más.

CodePen ya prepara esta estructura por nosotros.

Por eso, en el área HTML solo escribimos lo que va dentro de `body`.

```text
html
├── head → Información de la página
└── body → Contenido visible
```

# 6:30 – 7:40 | Atributos

Los elementos pueden tener información adicional.

Esa información se llama atributo.

Un atributo se escribe dentro de la etiqueta de apertura.

Tiene un nombre y un valor entre comillas.

Probemos con el atributo `title` en nuestro párrafo.

```html
<p title="Ciudad inca ubicada en Cusco, Perú">
  Machu Picchu es una antigua ciudad inca ubicada en Cusco, Perú.
</p>
```

Si colocamos el cursor sobre el párrafo y esperamos un momento, aparece un pequeño mensaje con ese texto.

Más adelante utilizaremos atributos para agregar imágenes y enlaces.

```text
<p title="Mensaje">
   ↑       ↑
 Nombre   Valor

Nombre + valor = Atributo
```

# 7:40 – 8:30 | Un título secundario

Una página puede tener varios títulos de distinta importancia.

El `h1` es el título principal. Normalmente se usa uno por página.

Para los títulos secundarios utilizamos `h2`.

```html
<h2>Conoce Machu Picchu</h2>
<p>
  Machu Picchu es una antigua ciudad inca ubicada en Cusco, Perú. Es uno de los destinos
  turísticos más conocidos del mundo.
</p>
```

Existen también `h3`, `h4`, `h5` y `h6`.

Mientras más grande es el número, menos importante es el título.

Por ahora, `h1` y `h2` son suficientes.

# 8:30 – 9:00 | Repaso rápido

Repasemos lo que aprendimos.

HTML le dice al navegador qué es cada parte del contenido.

Una etiqueta se escribe entre símbolos "menor que" y "mayor que".

Un elemento está formado por la etiqueta de apertura, el contenido y la etiqueta de cierre.

Una página tiene dos partes principales: `head` y `body`.

Un atributo agrega información adicional a un elemento.

```text
Etiqueta   → <p>
Elemento   → <p>Texto</p>
Atributo   → title="Mensaje"
```

# 9:00 – 9:40 | Reto práctico

Ahora es tu turno.

Crea una página sobre tu propio lugar favorito. Puede ser una ciudad, un parque, un restaurante o tu habitación.

Tu página debe tener:

```text
✓ Un título principal con <h1>

✓ Un párrafo con <p>

✓ Un título secundario con <h2>

✓ Otro párrafo con una descripción

✓ Un atributo title en uno de los párrafos
```

Pausa el video y practica en CodePen.

Si algo no se ve como esperabas, revisa que cada etiqueta de apertura tenga su etiqueta de cierre.

No te preocupes por el color o el diseño. De eso nos encargaremos más adelante con CSS.

# 9:40 – 10:00 | Cierre

¡Muy bien!

Acabas de crear tu primera página web.

En la siguiente lección agregaremos listas, imágenes y enlaces para que nuestra página sea mucho más completa.

¡Nos vemos allí!

---

# Descripción para YouTube

```text
Lección 2 de 6 — Introducción a HTML (10 min)

En esta lección aprenderás qué es HTML, cómo se escriben las etiquetas y los elementos, cómo es la estructura básica de una página y qué es un atributo.

No necesitas instalar nada. Solo tu navegador.

▶ Practica en CodePen (sin registro): [PEGAR_ENLACE_CODEPEN_LECCION_2]
📂 Código fuente: https://github.com/Mobvite/webdev-course-mobvite
   · Archivos de inicio: /starter-files/lesson-02
   · Ejemplo terminado: /completed-examples/lesson-02

Capítulos:
0:00 Introducción
0:40 ¿Qué es HTML?
1:50 Conociendo CodePen
2:30 Etiquetas y elementos
4:00 Nuestro primer párrafo
5:00 La estructura de una página HTML
6:30 Atributos
7:40 Un título secundario
8:30 Repaso rápido
9:00 Reto práctico
9:40 Cierre
```
