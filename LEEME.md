# Carta de presentación — AV Perú Corporation

**En línea:** https://dreeromer.github.io/avperu-presentacion/

Dos versiones del mismo diseño:

| Archivo | Para qué |
|---|---|
| `index.html` + `img/` + `fonts/` | La versión publicada. Carga rápido porque las fotos son archivos aparte. |
| `carta-offline.html` | Un solo archivo de 3.5 MB con todo dentro. Para USB, adjuntar por correo o presentar sin internet. |

Las fotos y las tipografías son locales: la página no pide nada a servidores
externos para mostrarse. La única salida a internet es el envío del formulario,
y solo cuando alguien lo usa.

## Datos de contacto

Ya están puestos en los dos archivos:

- Teléfono / WhatsApp: **+51 987 262 309**
- Correo: **comercial@grupoalvas.com**

No se muestra dirección ni enlace a la web (la web es esta misma página).

## El formulario de contacto

Al final de la página hay un formulario: nombre, correo o teléfono, y qué
necesita el cliente.

**Hoy, al enviarlo se abre WhatsApp con el mensaje ya escrito**, y además se
ofrece un enlace para mandarlo por correo. Se hizo así porque el envío directo
al correo (FormSubmit) manda un correo de activación a
comercial@grupoalvas.com la primera vez, y aún no hay acceso a esa bandeja.

### Para que los mensajes lleguen solos al correo

1. Busca en `index.html` esta línea, cerca del final:

       var ENVIO_POR_CORREO = false;

   Cámbiala a `true`. Haz lo mismo en `carta-offline.html`.
2. `git commit` y `git push`.
3. Abre la página publicada, llena el formulario y envíalo una vez.
4. Entra a **comercial@grupoalvas.com** y haz clic en el enlace de activación
   que llega de FormSubmit.
5. Desde ahí, cada mensaje llega solo a esa bandeja.

Si el envío por correo falla por cualquier motivo, el formulario cae de vuelta
en WhatsApp — no se pierde el contacto.

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
5. Desarrollo a medida — lo que se puede hacer fuera de las dos líneas
6. Control de salida — banda a todo lo ancho
7. Nuestra planta — recorrido lateral
8. Logística y entregas — recorrido entre unidades
9. Cobertura, entrega final y multidestino — tres datos de reparto
10. Cómo trabajamos — 4 pasos
11. Contacto y formulario

## Notas técnicas

- Los efectos son una mejora, no un requisito: si el JavaScript falla o está
  desactivado, la página se muestra como catálogo estático completo y legible.
- Respeta "reducir movimiento" del sistema: con esa preferencia activa se ve el
  mismo modo estático. Los tres estados están probados.
- Probado en escritorio (1512px) y móvil (420px), con el formulario en sus
  cuatro casos: campos vacíos, campo faltante, trampa antibots y envío válido.
- Publicada con GitHub Pages desde la rama `main`. Para actualizarla: editar,
  `git commit`, `git push` — el sitio se reconstruye solo en un par de minutos.
- Se agregaron `<meta charset>` y `<meta viewport>`, que faltaban. Sin el
  viewport el móvil dibujaba la página con ancho de escritorio.
- Peso en línea: 59 KB de HTML + 2.4 MB de fotos que llegan en paralelo.
