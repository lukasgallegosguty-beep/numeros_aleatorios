# Números Aleatorios

App móvil (PWA) para generar números aleatorios entre un mínimo y un máximo, con historial y funcionamiento sin conexión.

**Abrir la app:** https://lukasgallegosguty-beep.github.io/numeros_aleatorios/

## Qué hace

- Genera un número entero al azar entre el mínimo y el máximo (ambos incluidos; acepta negativos).
- Guarda un historial con fecha y hora, mínimo, máximo y número obtenido.
- Funciona sin conexión después de abrirla una vez con internet.
- Se adapta a teléfonos, tablets y computadores.

El historial se guarda en cada dispositivo (no se comparte entre teléfonos).

## Instalarla en el teléfono

1. Abre el enlace de arriba con conexión a internet.
2. **Android (Chrome):** menú ⋮ → *Agregar a pantalla principal* / *Instalar app*.
   **iPhone (Safari):** botón Compartir → *Agregar a inicio*.
3. Desde ese momento se abre desde el ícono, con o sin conexión.

## Archivos

| Archivo | Función |
|---|---|
| `index.html` | La app completa (interfaz, estilos y lógica) |
| `sw.js` | Service worker: guarda la app para uso sin conexión |
| `manifest.webmanifest` | Datos de instalación (nombre, íconos, colores) |
| `icons/` | Íconos de la app |

Al modificar la app, sube la versión de `CACHE` en `sw.js` (por ejemplo `aleatorios-v2`) para que los teléfonos descarguen la versión nueva.
