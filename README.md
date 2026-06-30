# Upsell TSL — Acompañamiento Musa Elite (Español)

Versión en español (neutro, natural para México, Colombia, EE. UU. hispano y España)
de la página de ventas del upsell "Acompañamiento Musa Elite". Estática,
autosuficiente, mobile-first. Misma identidad visual de la marca: fuente Inter,
rosa `#EC4899`, CTA verde, columna de lectura de 640px.

## Archivos
- `index.html` — la página completa (16 secciones)
- `styles.css` — sistema de diseño de la marca
- `script.js` — año dinámico del pie de página
- `garantia-30-dias-prompt.json` — prompt para generar el sello de garantía (en español)
- `assets/` — imágenes

## Precio configurado
**US$ 19 al mes (suscripción mensual recurrente).** Anclado contra el costo de un
entrenador personal (US$ 700–1,000/mes) y de una consultoría (US$ 1,500–2,000).
Para cambiarlo, edita el bloque `.price-callout` en `index.html`.

## ⚠️ QUÉ CAMBIAR ANTES DE PUBLICAR

### 1. Links de checkout (3 botones de compra)
Busca `<!-- CAMBIAR href por el link de checkout` en `index.html`.
Los 3 botones `.cta-btn` tienen `href="#"`. Reemplázalos por el link de aceptación del upsell.

### 2. Link de rechazo (2 links "No, gracias")
Busca `<!-- CAMBIAR href por la URL del downsell`. Hoy están en `href="#"`.

### 3. Sello de garantía (en español)
Genera el sello con `garantia-30-dias-prompt.json` (textos: GARANTÍA INCONDICIONAL /
30 DÍAS / SATISFACCIÓN GARANTIZADA) y guárdalo como `assets/garantia-30-dias.png`.
Mientras no exista, la página muestra automáticamente un sello CSS de respaldo ("30 DÍAS").

### 4. Imágenes de testimonios (placeholders)
Coloca los archivos reales en `assets/` con estos nombres (la página los toma solo):
- `roberta.jpg`, `daniela.jpg`, `patricia-antes.jpg`, `patricia-despues.jpg`, `murilo.jpg`

### 5. Badge de pago seguro
`assets/compra-segura.png` viene de la versión brasileña y puede mostrar "Pix"
(método solo de Brasil). Cámbialo por un badge de tarjetas/PayPal según tu mercado.

### 6. Páginas legales
El pie enlaza `privacidad.html`, `terminos.html`, `contacto.html` — crear/ajustar.

## Notas de localización
- Registro "tú", vocabulario neutro: "gimnasio" (no "academia"), "teléfono", "glúteos".
- Nombres de marca conservados: NalgasFlix, Musa Elite, Nalguitas, Murilo.
- Moneda en US$ (dólar) para público hispano internacional.

## Deploy
Estático (HTML/CSS/JS). Sube la carpeta a cualquier hosting estático o al builder del funnel.
