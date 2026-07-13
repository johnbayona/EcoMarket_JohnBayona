# EcoMarket 🌱

Tienda en línea de productos ecológicos, reutilizables y sustentables.
Maquetado con **HTML5 semántico y CSS3 puro** — cero JavaScript, cero frameworks.

## Descripción del proyecto

EcoMarket ofrece una plataforma accesible y atractiva donde los usuarios pueden
explorar productos sustentables, conocer sus beneficios y realizar compras
responsables. Este repositorio contiene, por ahora, la **Página de Inicio (Home)**.

## Cómo visualizarlo

No requiere instalación ni build. Basta con abrir `index.html` en el navegador,
o servirlo con cualquier servidor estático, por ejemplo:

```bash
# Opción 1: doble clic en index.html
# Opción 2: servidor local con Python
python3 -m http.server 8000
# luego visita http://localhost:8000
```

## Tecnologías utilizadas

- HTML5 semántico
- CSS3 puro (Flexbox, Grid, variables CSS, pseudo-clases `:checked`/`:hover`)
- Google Fonts (Fraunces + Work Sans)
- Sin JavaScript, sin librerías externas

## Estructura de archivos

```
EcoMarket/
├── css/
│   ├── main.css         # Reset, variables, tipografía
│   ├── layout.css       # Header, Footer, sistemas de grid
│   ├── components.css   # Cards, botones, inputs
│   └── animations.css   # Keyframes y transiciones
├── img/
│   ├── products/
│   ├── icons/
│   └── hero/
├── views/                # (próximas vistas: catálogo, nosotros, contacto)
├── index.html            # Home ✅
└── README.md
```

## Interactividad sin JavaScript

- **Filtros de categoría**: `<input type="radio">` ocultos + `<label>` visual,
  usando el selector `:checked + label`.
- **Favoritos (❤)**: `<input type="checkbox">` oculto que alterna entre un
  ícono de contorno y uno relleno con `:checked ~ label`.
- **Hover en tarjetas**: `transform: translateY()` + `box-shadow` en `:hover`.

## Capturas de pantalla

_Pendiente: agregar capturas móvil y escritorio antes de la entrega final._
