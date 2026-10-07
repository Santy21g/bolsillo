# Bolsillo

App web instalable (PWA) para registrar gastos mensuales desde el celular.

- Cargá cada gasto: monto, categoría, necesario / innecesario, detalle, fecha y medio de pago.
- Resumen del mes: total, gasto por día, comparación con el mes anterior y presupuesto.
- Barra de necesario vs. innecesario y ranking de categorías (tocá una para filtrar).
- Funciona sin conexión y se instala en la pantalla de inicio.
- Exportá el mes a CSV o descargá una copia completa (JSON) para respaldar o pasar a otro celular.

## Dónde se guardan los datos

En el `localStorage` del navegador del celular. No hay servidor ni cuenta: nadie más ve tus gastos, pero si borrás los datos del navegador se pierden. Hacé una copia desde **Ajustes → Descargar copia** cada tanto.

## Estructura

```
index.html            app completa (HTML + CSS + JS, sin dependencias)
sw.js                 service worker (modo offline)
manifest.webmanifest  datos para instalarla
icons/                íconos
netlify.toml          config de deploy
```

## Correrla local

```bash
python3 -m http.server 8000
```
