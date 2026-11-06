# Docs

Reglas para documentos de clase: avances de proyecto, prácticas y entregas. Todo lo que no cambia entre Docs y Presentaciones (paleta, familias, esquinas, nombre del alumno) está en el README general.

## Contenido

- Escribe en castellano, con frases directas y datos concretos: tiempos, frames, resoluciones, cantidades. Ejemplo: «El teaser dura 32 s a 24 fps (768 frames) y se monta con 11 divisiones.»
- Usa la primera persona del singular solo cuando el autor explica una decisión suya («Mi versión del storyboard usa modelos básicos en 3D en vez del típico boceto a lápiz»); en el resto, redacción impersonal.
- Abre cada apartado con lo esencial y deja lo provisional para una sección final de pendientes, como «Música y pendientes por cerrar».
- Las listas llevan una etiqueta en negrita seguida de dos puntos y el texto: «**Final:** corte a negro y créditos, sin título.»
- Sin emojis, sin signos de exclamación decorativos y sin adornos en el texto.

## Cabecera de la primera página

Todo documento académico abre con una cabecera en su primera página, sin portada aparte, en este orden:

1. Etiqueta superior en `doc-eyebrow`, una de `AVANCES DEL PROYECTO`, `PRÁCTICA` o `ENTREGA`.
2. Título en `doc-title`.
3. Subtítulo en `doc-subtitle` con el formato «Proyecto - descripción» (por ejemplo «Serie Mármol - Teaser de 32 s»), con la regla de `accent` de `stroke-accent` debajo, a `space-rule-pad`, y `space-header` antes del bloque de campos.
4. Tres campos, cada uno con la etiqueta en `doc-label` seguida de tres espacios y el valor en `doc-body`, con `space-field` debajo:
   - `ASIGNATURA`: nombre completo de la asignatura y, entre paréntesis, su sigla (por ejemplo «Proyecto intermodular de animaciones 3D, juegos y entornos interactivos (PrInAn3DJuEnIn)»).
   - `ALUMNO`: «Javier Echaide». En un documento académico se firma siempre «Javier», nunca el alias de usuario.
   - `CURSO`: «2X - Animación 3D, Juegos y Entornos Interactivos».

El contenido empieza justo debajo de los campos, en la misma página.

## Página y texto

- Formato A4 vertical, fondo `surface-page` y `margin-page` en los cuatro lados.
- Todo el texto va en `ink`. Párrafos en `doc-body` con `space-para` debajo.
- `accent` se reserva para la etiqueta superior, las etiquetas de campo, los subtítulos de bloque (`doc-label`), los H1 y la regla del subtítulo. Nunca para texto corrido, ni sobre `table-header`.
- `ink-muted` solo se usa en el subtítulo.

## Jerarquía de títulos

- H1: `doc-h1`, `accent`, `space-h1` arriba. Un apartado principal por tema («Resumen del teaser», «Necesidades gráficas»).
- H2: `doc-h2`, `ink`. Subapartado dentro de un H1.
- H3: `doc-h3`, `ink`. Solo si un H2 lo necesita.
- Subtítulos de bloque sueltos dentro de una sección (Personajes y props, Sets, Efectos y técnica): `doc-label` en `accent`, con `space-label` arriba, sin ser un nivel de título.

## Listas

- Viñetas ● para enumeraciones; sangría de 25 pt y 12 pt en la primera línea, `space-list` bajo cada elemento, texto en `doc-body`.
- Listas de pasos numeradas (prácticas y procedimientos): misma sangría y mismo espaciado, numeración decimal 1., 2., 3., y un paso por elemento, empezando por un verbo en infinitivo.
- Etiqueta en negrita y dos puntos al inicio de un elemento cuando el elemento responde a un tema («Historia:», «Música:»).

## Tablas

- Cabecera en `doc-body` negrita sobre `table-header`; bordes de celda en `table-rule` con `stroke-hairline`.
- Primera columna en negrita cuando es un identificador (número de plano, número de paso).
- Esquinas cuadradas (`radius-none`), sin sombreado alterno de filas y sin sombras.
- Anchos de columna fijos, con las columnas de datos cortos (Nº, Tiempo, Frames) estrechas y el texto largo en la última.
- Las imágenes de una tabla (miniaturas de un storyboard) van dentro de su celda, a ancho de columna, sin marco.

## Fundamentos visuales

- Sistema de un solo tema, claro, sobre página blanca: no hay modo oscuro.
- Dos familias: `serif` (Georgia) para título, subtítulo y encabezados; `sans` (Lato) para cuerpo, etiquetas y tablas. Los tamaños están dados en puntos en los estilos y en píxeles equivalentes en los tokens.
- Sin degradados, sombras, esquinas redondeadas ni iconos decorativos. La única regla de color del documento es la de `accent` bajo el subtítulo.
- Los enlaces se escriben en `accent` subrayados.

## Pendiente de definir

Esta parte cubre avances de proyecto, prácticas y entregas con cabecera en primera página. No define portada aparte, pies de figura, bloques de código ni notas destacadas; no los inventes: pregunta antes.
