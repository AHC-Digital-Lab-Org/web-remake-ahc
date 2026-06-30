# Web AHC — Rediseño Digital del Campus

Capa de **CSS y JavaScript personalizado** para la web institucional (WordPress/Divi) y el Campus
(Moodle/Edwiser) de la Asociación Huella de Carbono, según el *Plan de Acción: Rediseño Digital 2026*.

Es desarrollo web nativo (HTML/CSS/JS), no una SPA: el plan pide inyectar código para superar las
limitaciones de Divi y Edwiser, usando Vanilla JS, IntersectionObserver, diseño Bento y glassmorphism.

## Contenido

| Archivo | Función |
|:--|:--|
| `index.html` | Showcase del prototipo: Campus AHC, rejilla Bento, tarjetas y componentes interactivos. |
| `style.css` | Tokens de marca y estilos base. |
| `custom-style.css` | Rediseño avanzado: Bento, glassmorphism, componentes interactivos y modales. |
| `custom-interactions.js` | IntersectionObserver para revelar los elementos al hacer scroll. |
| `script.js` | Lógica de los componentes interactivos (tarjetas, drag & drop, vídeo, hotspots, quiz…). |
| `h5p-overrides.css` | Estilos para unificar los H5P embebidos en Moodle/WordPress con la identidad AHC. |
| `DEPLOYMENT_NOTES.md` | Guía de inyección de código en Divi y Edwiser. |
| `memoria_tecnica.md` | Memoria técnica del proyecto. |

## Uso

Abre `index.html` en el navegador para ver el prototipo. Está disponible en español y catalán
(selector de idioma en la cabecera).

## Despliegue

El CSS se inyecta en *Divi → Theme Options → Custom CSS* (y en el Custom CSS de Edwiser RemUI); el JS en
*Divi → Integration → body*, envuelto en `DOMContentLoaded`. `index.html` sirve como referencia visual del
resultado. Pasos detallados en [`DEPLOYMENT_NOTES.md`](DEPLOYMENT_NOTES.md).

## Autor

Jaber Al Abbadi — Asociación Huella de Carbono.
