# Presentaciones

Reglas para las diapositivas de exposiciones de clase. Paleta, familias y esquinas comunes: README general.

## Principios

- Una idea por diapositiva. Si necesitas explicar dos cosas, haz dos diapositivas.
- El título afirma algo («Bajar a 128 muestras reduce el render a un tercio del tiempo»), no nombra un tema («Resultados»). Va en frase normal, nunca en mayúsculas.
- La diapositiva es una prueba visual de lo que dices, no tu guion. No repitas en texto lo que ya dice el título; añade una frase o un pie solo si dan un dato nuevo.
- Prefiere una imagen, una tabla o un número real a una lista de viñetas. Los datos de la tabla y las cifras son siempre los del trabajo, nunca inventados.
- Antes de añadir más imágenes de las previstas, pregunta.

## Lienzo y rejilla

- 16:9, `slide-canvas-w` por `slide-canvas-h`. Un píxel equivale a un punto de PowerPoint, así que 24 px es 24 pt.
- Márgenes laterales `slide-margin`; el contenido mide 848 px de ancho.
- El título empieza siempre arriba a la izquierda, a `slide-top` del borde y a `slide-margin` del lateral, en todas las diapositivas.
- Dos columnas cuando hace falta: texto a `slide-col-text` desde el margen izquierdo, e imagen o pasos a `slide-col-side` desde x = 480 hasta el margen derecho.
- No hay cabecera. Solo hay pie, a `slide-footer` del borde inferior.

## Pie de página

- «Javier Echaide» a la izquierda y el número de diapositiva a la derecha, en `slide-small`.
- Sobre `surface-slide` va en `ink-muted-slide`; sobre `surface-ink`, en `text-muted-on-ink`.
- La portada lleva solo el nombre, dentro de su columna de texto. La imagen a pantalla completa lleva el número en su banda y no lleva nombre.

## Texto y color

- Cuatro tamaños, ninguno más: `slide-display` (portada, idea clave, cierre), `slide-title`, `slide-body` y `slide-small`. El cuerpo no baja de 24 px y nada baja de 18 px.
- Sobre `surface-slide`: texto en `ink`, texto secundario en `ink-muted-slide`, acento en `accent`. Sobre `surface-ink`: texto en `text-on-ink`, secundario en `text-muted-on-ink`, acento en `accent-on-ink`.
- El acento marca solo una cosa por diapositiva: una palabra clave, un número de paso, «Parte N» o «Fuentes». Nunca barras de color junto al texto, rellenos de acento ni más de un color de acento.
- Sin degradados, sombras, esquinas redondeadas ni emojis. Sin iconos que decoren: si un icono no explica algo, no va.

## Imágenes

- Son del propio trabajo: renders de Blender, capturas de pantalla, fotos propias. Nunca fotos de stock.
- Cada imagen enseña algo concreto y lleva un pie de figura corto («Fig. 1. Cada columna es la misma pieza, rotada.») en `slide-small` y `ink-muted-slide`, justo debajo.
- Mientras la imagen no está puesta, el hueco va en `table-header` sobre `surface-slide` y en `surface-ink-raised` sobre `surface-ink`, con una línea que dice qué imagen falta.

## Tipos de diapositiva

Son ocho. Elige el que corresponda a la idea; no los mezcles.

1. **Portada** (`surface-ink`). Imagen a la derecha, a sangre y de alto completo, en columna de 360 px desde x = 600. A la izquierda, título en `slide-display` a 500 px de ancho, y debajo «Asignatura · Exposición de proyecto» en `slide-body` y `accent-on-ink`.
2. **Sección** (`surface-ink`). «Parte N» en `slide-title` y `accent-on-ink`, y debajo el título de la parte en `slide-title` y `text-on-ink`, a 760 px de ancho. Sin número gigante ni imagen. Se numera «Parte 1», «Parte 2»… para no confundirlo con el número de diapositiva.
3. **Imagen con título** (`surface-slide`). Título en `slide-title` en la columna de texto; imagen de 424 × 366 px en la columna derecha y su pie de figura debajo. Sin más texto.
4. **Imagen a pantalla completa** (`surface-slide`). La imagen ocupa 960 × 444 px desde el borde superior; debajo, banda `surface-ink` de `slide-band` con el título en `slide-title` (una sola línea) y el número a la derecha en `slide-small`. Para renders o capturas que necesitan verse grandes.
5. **Pasos** (`surface-slide`). Título en la columna de texto. A la derecha, de tres a cuatro pasos, uno cada `slide-step-gap`, cada uno con línea `stroke-slide-rule` en `table-rule`, número 01, 02, 03 en `slide-title` y `accent`, y el texto en `slide-body`. Cada paso empieza con un verbo en infinitivo.
6. **Tabla** (`surface-slide`). Título a 848 px de ancho. Debajo, tabla de 560 px: cabecera en `slide-small-strong` sobre `table-header`, celdas en `slide-body` con borde inferior `stroke-slide-rule` en `table-rule`. A la derecha puede ir una nota en `slide-small` que diga de dónde salen los datos.
7. **Idea clave** (`surface-slide`). Solo una frase en `slide-display` y `ink`, a 848 px de ancho, con una palabra o expresión en `accent`. Sin texto debajo.
8. **Cierre** (`surface-ink`). Frase de conclusión en `slide-display` y `text-on-ink`, a 848 px. Debajo, «Fuentes» en `slide-small-strong` y `accent-on-ink`, y las fuentes en `slide-small` y `text-muted-on-ink`, con interlineado 1,5.

## Variantes por proyecto

Si un proyecto lo pide (por ejemplo, uno de Minecraft con su interfaz), se pueden cambiar los colores, los marcos y los iconos. La rejilla, los ocho tipos de diapositiva, las medidas y la tipografía de lectura (`slide-body`, `slide-small`) no cambian.

## Pendiente de definir

Animaciones y transiciones, la herramienta final (Canva o Google Slides) y los tipos de diapositiva de pregunta de apertura, vídeo e índice no están definidos; no los inventes: pregunta antes.
