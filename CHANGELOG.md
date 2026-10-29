# Registro de cambios

Todos los cambios notables de Zavitar se documentan en este archivo.

## [0.2.0] - 2026-10-28

### Añadido
- Apariencia: tema de la interfaz **Automático** (sigue al modo claro u oscuro de Windows), **Oscuro** o **Claro**, y transparencia de la rueda ajustable. Se abre desde la bandeja.
- Ventana de **Ajustes** desde la bandeja: calidad de conversión (**Alta**, **Equilibrada** o **Ligera**), carpeta de salida, plantilla de nombre de archivo y formato favorito de la rueda.
- Pausar y reanudar la cola desde la bandeja.
- Botón **Cancelar** en la ventana de progreso.
- Aviso al terminar con el botón «mostrar en la carpeta».
- PDF a imágenes: todas las páginas en una carpeta, o solo un rango de páginas.
- Varias imágenes en un solo PDF.
- DOCX a texto, PDF a DOCX (solo texto) y DOCX a PDF (requiere Microsoft Word instalado).
- Soltar una carpeta entera sobre la rueda: se convierten los archivos que contiene.

## [0.1.0] - beta inicial

Primera versión pública (beta).

### Añadido
- Conversión de archivos arrastrando un archivo, pulsando Mayús y eligiendo el formato en la rueda; la copia convertida aparece junto al original.
- Conversión de imágenes, audio, vídeo y PDF mediante FFmpeg y PDFium (opcionales; sin ellos esos formatos no aparecen en la rueda).
- Soporte de HEIC con las extensiones HEIF/HEVC de Microsoft Store (opcional).
- Icono en la bandeja con «Estado del sistema» y «Iniciar con Windows».
- Comprobación del sistema con `zavitar.exe --check` (códigos de salida 0, 1 y 2).
- Instalador de doble clic (por usuario, sin administrador) y paquete portátil `.zip` con `install.ps1` y `uninstall.ps1`.

### Limitaciones conocidas
- Un PDF de varias páginas convertido a imagen genera solo la primera página.
- Los GIF, WebP y AVIF animados, y los TIFF de varias páginas, se convierten a partir del primer fotograma o página.
- Los instaladores no están firmados con certificado de código: Windows SmartScreen mostrará un aviso.
- Solo Windows 10 (1809 o posterior) y Windows 11, de 64 bits.
