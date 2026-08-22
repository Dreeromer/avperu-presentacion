# Carta de presentación — AV Perú Corporation

**En línea:** https://dreeromer.github.io/avperu-presentacion/

Dos versiones del mismo diseño:

| Archivo | Para qué |
|---|---|
| `index.html` + `img/` + `fonts/` | La versión publicada. Carga rápido porque las fotos son archivos aparte. |
| `carta-offline.html` | Un solo archivo de 3.5 MB con todo dentro. Para USB, adjuntar por correo o presentar sin internet. |

Ninguna de las dos pide nada a servidores externos.

## Qué falta rellenar

Hay que hacerlo en **los dos** archivos (`index.html` y `carta-offline.html`).
Busca `data-slot` — son 4 líneas seguidas, cerca del final — y reemplaza el texto
entre corchetes:

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

- Los efectos son una mejora, no un requisito: si el JavaScript falla o está
  desactivado, la página se muestra como catálogo estático completo y legible.
- Respeta "reducir movimiento" del sistema: con esa preferencia activa se ve el
  mismo modo estático. Los tres estados están probados.
- Probado en escritorio (1440px) y móvil (414px).
- Publicada con GitHub Pages desde la rama `main`. Para actualizarla: editar,
  `git commit`, `git push` — el sitio se reconstruye solo en un par de minutos.
- Peso en línea: 43 KB de HTML + 2.4 MB de fotos que llegan en paralelo.
