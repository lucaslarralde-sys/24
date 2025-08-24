
# Instrucciones de carga de assets

## Logos
Reemplazá los placeholders manteniendo **el mismo nombre de archivo** y formato:

- `assets/img/ecowatt_logo.svg` — Logo ECOWATT (header)
- `assets/img/partners/fuchs.svg`
- `assets/img/partners/2g.svg`
- `assets/img/partners/aqana.svg`
- `assets/img/partners/daga.svg`
- `assets/img/partners/airclean.svg`

> Podés usar SVG (recomendado). Si tenés PNG, mantené el nombre pero extensión `.png` y actualizá el `src` en `index.html` si fuese necesario.

## Galería
Colocá 12 imágenes en:
```
assets/img/gallery/galeria_01.jpg
...
assets/img/gallery/galeria_12.jpg
```
Formato sugerido: JPG 4:3, ~1600×1200px.

## Video (Hero)
Ubicá el video en:
```
assets/video/hero-ecowatt.mp4
```
y asegurate que el `<source>` del `<video>` apunte a esa ruta.

---

## Color banda “Soluciones y tecnologías”
El color se controla con la variable CSS `--solutions-gray` en el `<style>` del HTML.

```
:root{
  --solutions-gray: #b8bdc5; /* TODO: reemplazar por gris exacto de la captura */
}
```

Reemplazá por el **hex exacto** de la captura cuando lo tengas.
