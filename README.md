# Sistema de diseño

Sistemas de diseño de Javier Echaide para documentos y presentaciones.

| Carpeta | Estado |
| --- | --- |
| `academico/` | Docs de clase (avances, prácticas y entregas) y presentaciones para exposiciones de clase. Definido. |
| `personal/` | Pendiente de definir. |

## Estructura de `academico/`

Usa el mismo formato que el lienzo de Claude:

| Archivo | Contenido |
| --- | --- |
| `tokens.json` | Colores, tipografías, espaciados y trazos. Los estilos de Docs llevan el prefijo `doc-` y los de Presentaciones, `slide-`. |
| `README.md` | Base común: paleta, familias y reglas generales. |
| `docs.md` | Reglas de los documentos A4. |
| `presentaciones.md` | Reglas de las diapositivas 16:9 y descripción de los 8 tipos. |
| `components/Cover/` | Portada del sistema. |
| `components/Doc*/` | Vistas previas de la cabecera y la tabla de un documento. |
| `components/Slide*/` | Una vista previa por cada tipo de diapositiva: portada, sección, imagen con título, imagen a pantalla completa, pasos, tabla, idea clave y cierre. |
