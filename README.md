# Zavitar

**Convierte cualquier archivo con un arrastre.** Programa gratuito para Windows (beta 0.2).

Arrastra un archivo, mantén **Shift** y suéltalo sobre el formato que necesitas en la rueda que aparece junto al cursor. Zavitar guarda la copia junto al original: sin abrir programas y sin subir nada a internet.

Página del programa: <https://rasec-dev.pages.dev/zavitar/>

## Descargar

Ve a [Releases](https://github.com/NotCronox/zavitar/releases/latest) y baja **`Zavitar-Setup-0.2.0.exe`**: doble clic y listo. Se instala solo para tu usuario, sin permisos de administrador.

También hay una versión portable (`Zavitar-0.2.0-win-x64.zip`) con scripts de instalación. Los hashes SHA256 están en `SHA256SUMS.txt`:

```powershell
Get-FileHash -Algorithm SHA256 .\Zavitar-Setup-0.2.0.exe
```

> Zavitar aún no tiene firma digital (es una beta). Windows puede mostrar «Windows protegió tu PC»: elige **Más información → Ejecutar de todos modos**. Algunos antivirus pueden avisar porque usa un gancho de teclado y ratón para detectar el arrastre.

## Requisitos

- Windows 10 (1809 o posterior) u 11, de 64 bits. No necesitas nada más.
- Opcional: las extensiones «HEIF» y «HEVC» de Microsoft Store para fotos HEIC; un codificador H.264 del equipo para video a MP4 (en ediciones N de Windows, el Media Feature Pack).

## Formatos

- **Imágenes:** JPG, PNG, WEBP, HEIC, AVIF, TIFF, BMP, GIF, SVG (como origen) y PDF.
- **PDF:** a PNG o JPG (primera página), a TXT, y de imagen a PDF.
- **Audio:** MP3, M4A, WAV, FLAC, OGG, OPUS.
- **Video:** MP4, MKV, WEBM, MOV, AVI, GIF y extracción de audio.

## Limitaciones de la beta

- Un PDF de varias páginas pasado a imagen genera solo la primera página.
- Aún no convierte documentos Word ni EPUB, ni tiene opciones de calidad.
- No funciona al arrastrar desde aplicaciones ejecutadas como administrador.
- HEIC necesita las extensiones de Microsoft Store (reinicia Zavitar tras instalarlas).

## Privacidad

Todo se procesa en tu equipo. Zavitar no se conecta a internet ni recoge datos.

## Licencias

Zavitar es gratuito y se ofrece tal cual, sin garantía (ver `LICENSE.txt`). Incluye **FFmpeg como programa independiente bajo licencia GPL** y otras librerías con sus propias licencias; los avisos y la oferta de código fuente de FFmpeg están en la carpeta `licenses` de la instalación y del zip.

Código fuente de FFmpeg: en cada release, `Zavitar-<versión>-ffmpeg-source.zip`; o bajo pedido a **cogjo0729@gmail.com**.

## English

Zavitar is a free Windows tray app (beta 0.2) that converts files by drag-and-drop: drag a file, hold Shift, drop it on a format in the wheel next to the cursor. Everything runs locally; nothing is uploaded. Download `Zavitar-Setup-0.2.0.exe` from [Releases](https://github.com/NotCronox/zavitar/releases/latest). Requires Windows 10 (1809+) or 11, 64-bit. Not code-signed yet, so Windows SmartScreen may warn. FFmpeg is bundled as a separate GPL program; FFmpeg source is available on request at cogjo0729@gmail.com.
