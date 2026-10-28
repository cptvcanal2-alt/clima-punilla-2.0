# Clima Punilla – Canal TV

Página estática (sin build) que arma las imágenes de clima para TV:

- **Clima localidades:** 11 localidades de Punilla y alrededores.
- **Pronóstico extendido:** Villa Carlos Paz, siempre los 3 próximos días (grande = mañana).

Datos de [Open-Meteo](https://open-meteo.com/). Todo se puede editar a mano desde el botón **✏️ Editar** y se baja como PNG de 1920×1080 con **⬇ Descargar**.

## Estructura

```
index.html
img/
  despejado.png  seminublado.png  nublado.png  lluvia.png
  llovizna.png   tormenta.png     niebla.png    nieve.png
  plantilla_sola.png        (fondo de localidades)
  plantilla_extendido.jpg   (fondo del extendido)
```

## Publicar en Vercel

1. Subir esta carpeta a un repo de GitHub (`index.html` e `img/` en la raíz).
2. En Vercel: **Add New → Project**, elegir el repo e **Deploy** (Framework Preset: *Other*, sin build command).
3. Cada commit a `main` redespliega solo.
