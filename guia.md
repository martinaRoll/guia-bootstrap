## ¿Qué es Bootstrap?

Es un framework de CSS y JS que te da estilos, componentes y una estructura responsive para hacer sitios web rápido y bien diseñados.
Evita escribir todo el CSS desde cero.

## Contenedores (.container y .container-fluid)

Todo en Bootstrap empieza dentro de un container.
Sirve para centrar y dar un ancho máximo al contenido.

Tipos:

    .container → ancho fijo, cambia según el tamaño de pantalla.

    .container-fluid → ocupa siempre el 100% del ancho.

## Sistema de grillas (Grid System)

El corazón de Bootstrap.
Funciona con filas (.row) y columnas (.col):

    <div class="container">
    <div class="row">
        <div class="col">Columna 1</div>
        <div class="col">Columna 2</div>
        <div class="col">Columna 3</div>
    </div>
    </div>

Bootstrap divide el ancho de la pantalla en 12 columnas.

## Clases y utilidades

Bootstrap funciona agregando clases en el HTML.

Colores: .text-primary, .bg-danger, .btn-success.

Espaciado:

- m = margin, p = padding.

Ej: .m-3 (margin 3), .p-2 (padding 2).

- Alineación: .text-center, .d-flex, .justify-content-between.
- Tamaños: .w-50 (ancho 50%), .h-100 (alto 100%).

## Componentes listos

Bootstrap trae bloques ya diseñados para usar:

- Botones:
  .btn btn-primary, .btn btn-outline-dark.
- Navbars (menús de navegación).
- Cards (tarjetas con contenido).
- Modals (ventanas emergentes).
- Forms (formularios con inputs estilizados).
