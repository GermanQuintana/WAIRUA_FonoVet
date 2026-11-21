# FonoVet by Wairua

Herramienta web para visualizar y medir fonocardiogramas a partir de la grabación de un fonendo digital. Es una sola página: no necesita servidor ni instalación, y el audio se procesa en el navegador sin enviarse a ningún sitio.

## Qué hace

- Carga audio o vídeo con audio (WAV, MP3, M4A, MP4), hasta 3 minutos.
- Dibuja el fonocardiograma con envolvente y el espectrograma de 0 a 1000 Hz.
- Filtros: corazón, corazón y soplos, soplos, pulmón o sin filtro.
- Estima la frecuencia cardiaca y marca los latidos contados. Las marcas se pueden corregir a mano (añadir, quitar, ÷2, ×2).
- Permite eliminar zonas de ruido, recortar y guardar tramos como muestras reproducibles.
- Genera un informe en PDF con datos del veterinario, del paciente y del registro.

## Qué no hace

No detecta ni clasifica soplos y no emite diagnósticos. El informe es informativo y debe valorarse junto con la exploración física, la historia clínica y las pruebas complementarias.

## Uso

Abre `index.html` desde un servidor web (por ejemplo GitHub Pages, o `python3 -m http.server` en esta carpeta). Abierto directamente como archivo local funciona, pero el logo puede no aparecer en el PDF.

Las muestras guardadas viven solo mientras la página está abierta.

## Dependencias

Se cargan desde CDN: [jsPDF 2.5.1](https://github.com/parallax/jsPDF) para el PDF y las fuentes IBM Plex de Google Fonts. El resto es JavaScript sin librerías.

## Archivos

- `index.html`: la aplicación completa (HTML, CSS y JavaScript).
- `logo.png`, `logo-blanco.png`: logo de Wairua para fondo claro y oscuro.

© Wairua Veterinary Precision Medicine, S.L.U. Todos los derechos reservados.
