# Reglas del proyecto

## Sobre el proyecto

Página personal de Juan Esteban Martínez con links a redes sociales (Instagram, TikTok, YouTube) y a su marca WALKA. Un solo archivo `index.html` con CSS y JS inline. Desplegada en GitHub Pages con dominio propio (ver `CNAME`).

## Comunicación

- Hablamos en español.
- Antes de cambios grandes (rediseños, reestructurar el HTML, agregar librerías), muéstrame el plan primero y espera confirmación.
- Cambios pequeños y ajustes visuales: puedes aplicarlos directo y me cuentas qué hiciste.
- Si te paso un link de referencia, la idea es inspirarse en el estilo/animaciones y adaptarlo al propósito de esta página (links), no copiar literal.

## Stack técnico

**Permitido:**
- HTML, CSS y JavaScript vanilla.
- Google Fonts por `<link>`.
- SVGs inline.
- Librerías específicas vía CDN cuando una animación o efecto lo justifique (ej. GSAP, Lenis, Motion One). Preferir las más livianas.
- APIs externas desde el navegador si aportan valor.

**Prohibido:**
- Frameworks (React, Vue, Svelte, etc.).
- Bundlers ni build step (Vite, Webpack, etc.).
- `npm install` / `package.json` / `node_modules`.
- Backend propio o cualquier cosa que requiera servidor.

## Restricciones de despliegue

- Todo debe funcionar abriendo `index.html` directamente en el navegador.
- Despliegue: GitHub Pages estático. Sin GitHub Actions ni pipelines.
- Las rutas a assets deben ser relativas (no absolutas al root del dominio) para que funcione en cualquier entorno.

## Rendimiento

- Mantener la página ligera. Es una landing de links, no una app.
- Evitar imágenes sin optimizar. Si agregamos assets nuevos, revisar peso.
- Antes de agregar una librería por CDN, evaluar si el efecto se puede lograr con CSS/JS vanilla.
- Priorizar First Paint rápido sobre efectos cargados al inicio.

## Convenciones de código

- Mantener todo en `index.html` mientras sea manejable. Si el archivo crece mucho, propondremos extraer CSS/JS a archivos separados.
- Comentarios en CSS con el estilo actual (`/* ── Sección ────── */`) para separar bloques.
- Variables CSS en `:root` para colores y tokens reutilizables.
