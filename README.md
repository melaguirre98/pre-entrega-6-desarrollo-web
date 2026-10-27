# Cafetería Origen

**Sitio publicado:** https://melaguirre98.github.io/pre-entrega-6-desarrollo-web/

Sitio web de una cafetería de especialidad, desarrollado en el curso de Desarrollo Web.

## Páginas
- `index.html`: inicio, con galería (carousel) y horarios (modal)
- `pages/servicios.html`: menú y preguntas frecuentes
- `pages/proyectos.html`: sucursales
- `pages/sobre-mi.html`: sobre nosotros
- `pages/contacto.html`: contacto

## Tecnologías
HTML5 semántico, SCSS (partials, variables, mixins con parámetros, `@extend`, `@for` y nesting), CSS Grid, Flexbox, Bootstrap 5.3 y AOS (animaciones al hacer scroll) por CDN, y Git/GitHub.

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
