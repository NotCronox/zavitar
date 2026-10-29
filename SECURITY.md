# Política de seguridad

## Versiones con soporte

Solo se corrigen fallos de seguridad en la última versión publicada de Zavitar.

| Versión | Soporte |
|---|---|
| 0.2.x | Sí |
| < 0.2 | No |

## Cómo reportar una vulnerabilidad

**No abras un issue público** para reportar una vulnerabilidad. Envía un correo a:

**cogjo0729@gmail.com**

Incluye, si puedes:

- La versión de Zavitar y la versión de Windows.
- Los pasos para reproducir el problema, o un archivo de prueba que lo muestre.
- El impacto que crees que tiene.

Intentaremos responder en un plazo de 7 días. Si el reporte se confirma, coordinaremos con quien lo envió la fecha de publicación de la corrección.

## Alcance

Zavitar convierte archivos con los permisos del usuario que lo ejecuta. Las conversiones corren en procesos aislados con límites de memoria y de tiempo, pero **no son un sandbox de seguridad completo** y no tienen aislamiento de red. Evita convertir archivos de origen no fiable en equipos con datos sensibles. Los fallos de este tipo que se describan con un archivo concreto son bienvenidos.

Los binarios de terceros (FFmpeg, PDFium) se descargan con versión y SHA-256 fijados; si detectas un problema en ellos, avísanos y también a su proyecto.
