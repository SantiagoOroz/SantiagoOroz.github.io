# santiagooroz.github.io

Portfolio de **Santiago Oroz** — Ingeniero de Inteligencia Artificial.
Río Grande, Tierra del Fuego, Argentina.

**En vivo:** https://santiagooroz.github.io/

---

## Qué es

Sitio de una sola página, orientado a empresas: qué problemas resuelvo, ocho casos
reales con su detalle técnico, stack, trayectoria y contacto. **Bilingüe español / inglés.**

## Cómo está hecho

HTML, CSS y JavaScript a mano. **Sin frameworks, sin build, sin dependencias** —
salvo las tipografías de Google Fonts. Se publica solo con hacer push a `main`.

| Archivo | Qué es |
|---|---|
| `index.html` | El sitio completo: estructura, estilos y scripts |
| `logo.png` | Marca personal (montañas y llama). Se pinta con máscara CSS, así toma el color de acento y sirve en ambos temas |
| `favicon.png` | La misma marca, ya coloreada, para la pestaña |
| `logomejore*.png` | Archivos fuente originales de la marca |
| `santiago-oroz.jpg` | Retrato del hero (880×1100) |
| `santiago-oroz-charla.jpg` | Banda a todo el ancho — presentando en el Samsung Innovation Campus |
| `powerbiinteractivo.png` | Tablero de Power BI entregado a Newsan |
| `org-*.png` · `org-*.jpg` | Logos de UTN, Centro Politécnico y El Dorado SRL, en la trayectoria |
| `CV-Santiago-Oroz-ES.pdf` · `CV-Santiago-Oroz-EN.pdf` | CV descargable, según el idioma activo |

> Los nombres de archivo se mantienen en ASCII a propósito: un acento en el nombre
> obliga a codificar la URL y se rompe fácil al servirlo.

### Detalles de implementación

- **Bilingüe** sin recargar: los dos idiomas viven en el HTML y se muestra uno por CSS
  (`html[lang]` + `data-l`). Arranca en el idioma del navegador y recuerda la elección.
- **Tema claro y oscuro** por tokens CSS: sigue al sistema y el visitante puede forzarlo.
- **Hero animado:** isolíneas dibujadas con marching squares sobre canvas, como una carta
  batimétrica a la deriva. Se congela cuando el hero sale de pantalla y no se anima si el
  visitante pidió menos movimiento.
- **Edad calculada** desde la fecha de nacimiento — nunca queda desactualizada.
- **Accesibilidad:** HTML semántico, foco visible, casos desplegables con `<details>`
  (funcionan sin JavaScript) y `prefers-reduced-motion` respetado.
- **SEO:** Open Graph y JSON-LD `schema.org/Person`, para que buscadores y asistentes
  de IA lean el perfil correctamente.

## Trabajo local

No necesita servidor: abrí `index.html` en el navegador. Para probarlo servido:

```bash
python -m http.server 8000
```

## Pendiente

Los dos PDFs del CV son de diciembre de 2025: no incluyen Tech del Fuego, la beca del
ITBA ni la IAthon. Conviene regenerarlos.

## Licencia

El código es libre de reutilizar. El contenido, las imágenes y la marca personal
son de Santiago Oroz.
