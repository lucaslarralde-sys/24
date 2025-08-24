
# ECOWATT — Sitio estático (GitHub + Netlify)

Este repo contiene la versión **estática** del sitio ECOWATT listo para publicar.

## Estructura
```
├── index.html
├── 404.html
├── netlify.toml
├── LICENSE
├── .gitignore
├── README.md
└── assets/
    ├── img/
    │   ├── ecowatt_logo.svg
    │   └── partners/ (colocar logos)
    └── video/
        └── hero-ecowatt.mp4  (agregá el video aquí)
```

> **Importante:** reemplazá los placeholders por tus archivos reales (logos y video). El `index.html` ya está **reordenado** en el orden solicitado y la banda de **Soluciones y tecnologías** usa **gris oscuro**.

---

## Cómo publicar en GitHub Pages (opcional)
1. Crear un repo nuevo en GitHub (por ejemplo `ecowatt-site`).
2. Subir todos los archivos de esta carpeta a la raíz del repo.
3. En *Settings → Pages*, elegir **Deploy from a branch** y **Branch: main / root**.
4. Guardar. La URL quedará disponible en unos minutos.

> GitHub Pages sirve archivos estáticos. Si preferís usar tu dominio y CDN optimizada, usá Netlify 👇.

---

## Cómo publicar en Netlify (recomendado)
1. Crear cuenta en https://app.netlify.com/.
2. **New site from Git** → conectar con GitHub → seleccionar el repo.
3. Build command: *(vacío)* &nbsp;&nbsp;•&nbsp;&nbsp; Publish directory: `.`
4. Deploy. Netlify asignará una URL del tipo `https://xxxxx.netlify.app`.
5. Para dominio propio: *Site settings → Domain management → Add domain*.
6. El archivo `netlify.toml` ya agrega headers de seguridad y caché para `/assets/*`.
7. Si subís el video a `/assets/video/hero-ecowatt.mp4`, se servirá directamente sin build.

---

## Personalizaciones frecuentes
- **Mapa en Contacto:** inserta tu iframe de Google Maps en la sección `#contacto`.
- **SEO:** ajusta `<title>` y la meta `description`.
- **Favicons:** agrega `/assets/img/favicon.ico` y referencias en `<head>`.
- **Analitycs:** pega tu script antes de `</body>`.

---

## Desarrollo local (opcional)
Podés abrir `index.html` directo en el navegador o correr un server simple:

```bash
# Python 3
python -m http.server 5173
# Luego: http://localhost:5173
```

---

## Licencia
MIT © ECOWATT


---

Para cargar logos e imágenes, seguí **ASSETS_INSTRUCCIONES.md**.
