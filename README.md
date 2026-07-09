# morfo

Sitio del estudio de diseño web **morfo** — dos hermanos, Costa Rica.

## Páginas
- `index.html` — landing principal (hero, proyectos, nosotros, contacto)
- `blue-zones/index.html` — proyecto Blue Zones Nicoya
- `nantipa/index.html` — proyecto Nantipa
- `404.html` — página de error

## Cómo verlo localmente
Es HTML/CSS/JS estático, sin build. Levantá un servidor simple desde esta carpeta:

```bash
python3 -m http.server 4242
```

Y abrí http://localhost:4242

## Hosting
Desplegado en **Vercel**. Toda la configuración (URLs limpias, redirects de las
URLs viejas `.html`, security headers y CSP) vive en `vercel.json`.
Si algún día se migra a Netlify, hay que trasladar esos headers/redirects a
archivos `_headers` y `_redirects`.

## Formulario de contacto
El formulario envía a Formspree; el endpoint está en el atributo `action`
del `<form>` en `index.html`. Sin JavaScript el formulario también funciona
(envío nativo a Formspree con validación del navegador).

## Estructura
- `assets/brand/` — favicons, iconos de app y marca
- `assets/fonts/general-sans/` — General Sans (solo las variantes Variable y Regular que usa el sitio)
- `assets/images/og/` — imágenes para redes sociales (1200×630)
- `assets/images/projects/` — capturas de los proyectos
