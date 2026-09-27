# tarjeta-sienna

Sitio web estático de una sola página, instalable como PWA (app) en el celular.

## Archivos

- `index.html` — la aplicación completa (HTML, CSS y JS embebidos). No hay backend ni build.
- `manifest.webmanifest` — metadata de la PWA (nombre, iconos, colores) para poder "Agregar a inicio".
- `sw.js` — service worker: cachea la app para que abra rápido y funcione sin conexión.
- `icons/` — iconos de la app (192, 512, apple-touch-icon).

## Funciones clave

- **Historial de consultas** (sección Medicamentos): cada consulta guardada queda como tarjeta colapsable (clic para expandir/contraer). El formulario de abajo permite cargar fecha, medicamentos, indicaciones y próxima cita, y "Guardar consulta" la agrega al historial.
- **Recordatorio de próxima cita**: al guardar una consulta con fecha de "próxima cita", se crea/actualiza automáticamente un recordatorio. Si dan permiso de notificaciones (botón dentro de 🔔 Recordatorios), el navegador muestra una notificación del sistema cuando falten 3 días o menos — solo mientras la app esté abierta o se abra ese día (no hay servidor para notificaciones push reales).
- **Instalar como app**: desde el navegador móvil, "Agregar a pantalla de inicio" / "Instalar app".

## Repositorio

https://github.com/lfranciscowa/tarjeta-sienna
