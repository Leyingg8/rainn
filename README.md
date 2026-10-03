# Rain or Shine Roofing and Restoration

Landing page estática para **Rain or Shine Roofing and Restoration** (San Diego County).
Un solo archivo `index.html` — sin build, sin dependencias, sin framework.

## Estructura

```
rain-or-shine/
├── index.html          ← toda la página (HTML + CSS + JS van aquí dentro)
├── assets/             ← logo, fotos de trabajo, badges y certificados
├── .gitignore
├── DESIGN.md           ← sistema de diseño (colores, tipografía, spacing)
├── README.md
└── PENDIENTE-formspree.md  ← pasos pendientes para activar el formulario
```

## Subir a GitHub

Opción 1 — sin instalar nada:

1. Entra a [github.com/new](https://github.com/new) y crea el repo (vacío, sin README).
2. Sube el contenido de esta carpeta arrastrándola a la pestaña *Add file → Upload files*.

Opción 2 — con Git instalado:

```bash
cd rain-or-shine
git init
git add .
git commit -m "Landing page Rain or Shine Roofing"
git remote add origin https://github.com/TU-USUARIO/TU-REPO.git
git push -u origin main
```

## Desplegar en Vercel

Opción 1 — desde la interfaz: importa el repo en [vercel.com](https://vercel.com).
Vercel detecta `index.html` automáticamente, no hay nada que configurar.

Opción 2 — sin cuenta de Git: en Vercel usa *Add New → Project* y sube el ZIP
`rain-or-shine-web.zip`.

Opción 3 — desde terminal:

```bash
npm i -g vercel
vercel
```

## Notas técnicas

- **Tailwind vía CDN** — se carga desde `cdn.tailwindcss.com` con la config definida
  dentro de `<script id="tailwind-config">`. Es lo más rápido para un sitio estático,
  pero **no es para producción a largo plazo**: Tailwind avisa que el CDN es solo
  para desarrollo. Si el sitio crece, conviene compilar Tailwind con un build.
- **Fuentes** — Montserrat y Open Sans desde Google Fonts, Material Symbols para iconos.
- **Imágenes** — todas locales en `assets/` (logo, fotos de trabajo, badge y
  certificado IICRC). No hay links externos que puedan expirar.
- **Header** — barra sticky de apartados con menú hamburguesa en móvil
  (`#menu-toggle` / `#mobile-nav`, JS al final del archivo).
- **Logo** — `assets/logo.png`, 1400×871 px (2x del tamaño máx. en pantalla).
  No redimensionarlo con paleta indexada: GDI+/WPF no respetan la paleta y
  corrompen los colores.
- **Animaciones** — `IntersectionObserver` con `data-stagger` para el escalonado.
  Todo respeta `prefers-reduced-motion`.
- **Videos** — `#video-section` usa iframes directos a
  `youtube-nocookie.com/embed/...` (sin JS). Probarlos siempre por `http://`,
  nunca abriendo `index.html` con doble clic: con `file://` YouTube rechaza el
  embed por falta de `Referer` (error 153 "Video player configuration error").
  Los cuatro clipes son verticales (9:16) de 27s, 28s, 11s y 15s.
- **Servidor local para previsualizar** (PowerShell, sin instalar nada):

  ```powershell
  powershell -NoProfile -ExecutionPolicy Bypass -File "%TEMP%\rain-server.ps1"
  ```

  Sirve el proyecto en `http://localhost:8080/`.

## Pendientes antes de publicar

1. Reemplazar `TU_ID_DE_FORMSPREE` por el ID real del formulario
2. Configurar el destinatario en Formspree → `eric@rainorshineroofingsd.com`
3. Agregar `og:image` (preview al compartir el link) y apuntar el dominio propio
4. Cuando se emita la licencia CSLB, agregar el número real en el footer
