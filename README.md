# Propuesta Digital — Centro Integral del Dolor

Landing page de propuesta comercial para Centro Integral del Dolor, San Pedro Sula, Honduras.

## Estructura del repositorio

```
/
├── index.html        # Landing page principal (~44KB)
├── hero.jpg          # Imagen hero (agenda automática)
├── embudo.jpg        # Sección embudo digital
├── whatsapp.jpg      # Sección WhatsApp + IA
├── medico.jpg        # Imagen final (médico + deportista)
├── netlify.toml      # Headers de caché para Netlify
└── README.md
```

## Deploy

Conectado a Netlify via GitHub. Cada push a `main` despliega automáticamente.

## Optimizaciones de rendimiento

- Imágenes externas (no base64) → carga en paralelo
- Hero image con `fetchpriority="high"` → LCP óptimo
- Imágenes secundarias con `loading="lazy"` → no bloquean render
- Google Fonts cargadas de forma no bloqueante
- Cache headers: imágenes en 1 año, HTML siempre fresco
- HTML: ~44KB (vs 930KB versión anterior)

