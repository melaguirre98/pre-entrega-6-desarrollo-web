# Cafetería Origen

**Sitio publicado:** https://melaguirre98.github.io/pre-entrega-6-desarrollo-web/

Sitio web de una cafetería de especialidad, desarrollado en el curso de Desarrollo Web.

## Páginas
- `index.html`: inicio, con galería (carousel) y horarios (modal)
- `pages/menu.html`: menú y preguntas frecuentes
- `pages/sucursales.html`: sucursales
- `pages/sobre-nosotros.html`: sobre nosotros
- `pages/contacto.html`: contacto

## Tecnologías
HTML5 semántico, SCSS (partials, variables, mixins con parámetros, `@extend`, `@for` y nesting), CSS Grid, Flexbox, Bootstrap 5.3 y AOS (animaciones al hacer scroll) por CDN, y Git/GitHub.

## SEO y accesibilidad
- Un `<h1>` propio por página, jerarquía de títulos correcta y `<title>` y `meta description` únicos.
- Todas las imágenes con `alt` descriptivo y nombres de archivo representativos.
- Contraste de color de texto verificado (mínimo 4,5:1) y enlace para saltar al contenido.

## Estructura de estilos
Todo el CSS propio nace de los archivos `.scss`. `css/style.css` es solo el resultado de la compilación.

```
scss/
├── main.scss              # único punto de entrada (solo @use)
├── utilities/             # _variables.scss, _mixins.scss
├── base/                  # _tipografia.scss, _base.scss
├── layout/                # _header.scss, _nav.scss, _grid.scss, _footer.scss
└── components/            # _buttons.scss, _cards.scss, _sucursales.scss,
                           # _carousel.scss, _modal.scss, _accordion.scss
```

## Cómo compilar
Con [Sass](https://sass-lang.com/install) instalado (`npm install -g sass`):

```
sass --no-source-map scss/main.scss css/style.css
```

Para recompilar automáticamente al guardar:

```
sass --watch --no-source-map scss/main.scss:css/style.css
```
