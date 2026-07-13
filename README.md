# EcoMarket 🌱

Tienda en línea de productos ecológicos, reutilizables y sustentables.
Maquetado con **HTML5 semántico y CSS3 puro** — cero JavaScript, cero frameworks.

## Descripción del proyecto

EcoMarket ofrece una plataforma accesible y atractiva donde los usuarios pueden
explorar productos sustentables, conocer sus beneficios y realizar compras
responsables. El repositorio contiene las 4 vistas principales: **Inicio**,
**Productos (Catálogo)**, **Sobre Nosotros** y **Contacto**.

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
├── views/
│   ├── productos.html     # Catálogo ✅
│   ├── sobre-nosotros.html # Brand Story ✅
│   └── contacto.html      # Contacto ✅
├── index.html             # Home ✅
└── README.md
```

## Interactividad sin JavaScript

- **Filtros de categoría**: `<input type="radio">` ocultos + `<label>` visual,
  usando el selector `:checked + label`.
- **Favoritos (❤)**: `<input type="checkbox">` oculto que alterna entre un
  ícono de contorno y uno relleno con `:checked ~ label`.
- **Hover en tarjetas**: `transform: translateY()` + `box-shadow` en `:hover`.
- **Favoritos del catálogo**: `<a href="#fav-N" id="fav-N">` + pseudo-clase
  `:target`, para practicar una técnica distinta a la del Home.
- **Carrusel de testimonios**: `scroll-snap-type` + anclas (`<a href="#slide-N">`)
  que desplazan el contenedor sin JavaScript.
- **Validación del formulario de contacto**: `:invalid` / `:valid` combinadas
  con `:not(:placeholder-shown)` para no marcar en rojo un campo vacío que
  el usuario aún no ha tocado.
- **Sidebar sticky del catálogo**: `position: sticky` para que acompañe el scroll.

## Capturas de pantalla

_Pendiente: agregar capturas móvil y escritorio antes de la entrega final._
