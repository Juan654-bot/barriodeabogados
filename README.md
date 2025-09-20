# Barrio de Abogados – Landing estática

Este paquete incluye una landing **lista para subir** a cualquier hosting estático (Vercel, GitHub Pages, Netlify, S3/CloudFront, etc.).

## Estructura
```
barrio-abogados-site/
├─ index.html        # archivo principal (Tailwind via CDN)
├─ img/
│  └─ hero.svg       # imagen de portada (reemplazar por foto real)
└─ docs/
   ├─ presentacion.pdf
   ├─ precios.pdf
   └─ contrato.doc
```

## Personalización rápida
- Editá en `index.html`:
  - `EMAIL_CONTACTO` y `WHATSAPP`
  - Reemplazá `img/hero.svg` por una foto real
  - Si cambiás los PDFs o sus rutas, actualizá los links en la sección **Descargas**

## Publicar en Vercel
1. Subí esta carpeta a un repo en GitHub.
2. En Vercel, **New Project** → importá el repo → Framework: *Other* → root `/`.
3. Deploy. ¡Listo!

## Publicar en GitHub Pages
1. Subí la carpeta al repositorio (rama `main`).
2. En **Settings → Pages**, seleccioná `Deploy from a branch` → rama `main` y carpeta `/ (root)`.
3. Guardá y esperá a que se publique.

## Notas
- Los valores de precios/cuotas son orientativos y deben sincronizarse con la última versión de la planilla.
- El formulario usa enlaces `mailto:` y `WhatsApp` (sin backend).
- Para un formulario con backend (Formspree, EmailJS, etc.), se puede integrar fácilmente en el futuro.
