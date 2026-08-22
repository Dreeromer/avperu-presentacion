# Carta de presentación — AV Perú Corporation

Página web de una sola pieza. `index.html` es **autónomo**: fotos y tipografías van
incrustadas dentro del archivo, no pide nada a internet. Funciona con doble clic,
desde un USB o sin conexión.

## Qué falta rellenar

Abre `index.html` en cualquier editor de texto, busca `data-slot` (son 4 líneas
seguidas, cerca del final) y reemplaza el texto entre corchetes:

    <li><b>Teléfono</b><span data-slot>[ teléfono ]</span></li>
    <li><b>Correo</b><span data-slot>[ correo ]</span></li>
    <li><b>Web</b><span data-slot>[ web ]</span></li>
    <li><b>Dirección</b><span data-slot>[ dirección ]</span></li>

Ejemplo: `<span data-slot>+51 999 999 999</span>`

## Correcciones aplicadas al PPT original

| PPT | Web |
|---|---|
| AV PERU COORPORATION | AV Perú Corporation |
| Merchandaising | Merchandising |
| Clasico / Premuim | Clásica / Premium |
| Logistica / Gestion | Logística / Gestión |
| "entrega dela guía" | "entrega de la guía" |

## Secciones

1. Portada — vitrina 3D de producto
2. Quiénes somos
3. Línea Clásica — carrusel cilíndrico 3D
4. Línea Premium — mesa de kits
5. Control de salida — banda a todo lo ancho
6. Nuestra planta — recorrido lateral
7. Logística integral — recorrido entre unidades
8. Cómo trabajamos — 4 pasos
9. Contacto

## Notas técnicas

- Respeta "reducir movimiento" del sistema: sin esa preferencia activa se ven los
  efectos; con ella, la página se lee como catálogo estático. Ambos estados están probados.
- Probado en escritorio (1440px) y móvil (414px).
- Peso: 3.5 MB. Para publicarla en web conviene subirla tal cual (GitHub Pages,
  Netlify o el hosting propio); no necesita carpeta de imágenes.
