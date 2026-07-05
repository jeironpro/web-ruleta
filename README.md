# Web Ruleta

Ruleta interactiva en una sola pagina. Configura numeros o nombres personalizados desde el panel lateral y haz girar la ruleta.

## Caracteristicas

- **Dos modos de configuracion**: Numeros (rango personalizable con opcion de incluir 0) o Nombres (anyade nombres, cada uno es un segmento)
- **Panel lateral flotante**: Se abre/cierra desde el boton flotante en la esquina superior derecha
- **Ruleta animada**: Dibujada con Canvas, animacion con desaceleracion natural
- **Responsive**: Funciona en dispositivos moviles y desktop
- **HTML semantico**: Estructura accesible y limpia
- **CSS moderno**: Flexbox, Grid, Custom Properties, Media Queries
- **JavaScript ES6+**: Modulos, clases, Canvas API

## Stack

- HTML5 semantico
- CSS3 (Flexbox, Custom Properties, Media Queries)
- JavaScript ES6+ (modulos, Canvas API)
- Sin bundlers ni frameworks

## Uso

Abrir `index.html` en un navegador o servir con un servidor local:

```bash
# Python
python -m http.server 8000

# Node
npx serve .
```

### Como funciona

1. Abre el panel lateral con el boton de ajustes (esquina superior derecha)
2. Elige el modo "Numeros" o "Nombres"
3. Configura los valores y presiona "Aplicar"
4. Presiona "Girar" para hacer girar la ruleta
5. El resultado se muestra debajo de la ruleta

## Estructura del proyecto

```
web-ruleta/
├── index.html           # Pagina principal (onepage)
├── favicon.svg          # Icono SVG de la ruleta
├── favicon.ico          # Icono fallback
├── robots.txt           # Configuracion para crawlers
├── sitemap.xml          # Mapa del sitio
├── css/
│   ├── reset.css        # Normalizacion de estilos
│   ├── variables.css    # Custom properties (colores, espacios, etc.)
│   └── style.css        # Estilos globales y de componentes
├── js/
│   ├── app.js           # Entry point
│   ├── modules/
│   │   ├── roulette.js  # Logica de la ruleta (Canvas, animacion, giro)
│   │   └── sidebar.js   # Panel lateral de configuracion
│   └── utils/
│       └── dom.js       # Helpers de DOM ($, $$)
└── assets/
    └── images/          # Imagenes del proyecto
```

## Reglas del proyecto

- No se usa `innerHTML` ni ninguna inyeccion insegura de HTML
- CSS con media queries para responsive
- HTML con estructura semantica
- Comentarios en espanol en el codigo
- Iconos de Material Symbols en lugar de emojis
- ESLint + Stylelint + Prettier para calidad de codigo

## Licencia

MIT
