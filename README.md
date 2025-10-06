## ¿Qué es Bootstrap?

Bootstrap es un **framework de CSS y JavaScript** que permite diseñar sitios web rápidos, modernos y adaptables (responsive) sin tener que escribir todos los estilos desde cero.
Su principal característica es que funciona a través de clases CSS ya predefinidas y un sistema de grilla que organiza el contenido.

## Cómo usar Bootstrap

Podés incluirlo de dos formas:

**1. 🔗 Vía CDN (la más rápida y usada)**

Copiar y pegar dos links:

    <!-- Antes de </head> -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">

    <!-- Antes de </body> -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>

**2. 📦 Descargando los archivos**

Podés descargar Bootstrap desde su web oficial y linkear los archivos CSS y JS desde tus carpetas locales.

## Clases

En Bootstrap todo se hace con clases (class="...").

Ejemplo:

    <button class="btn btn-primary">Botón azul</button>
    <p class="text-center">Texto centrado</p>

Cada clase aplica un estilo o comportamiento, sin escribir CSS manualmente.
Esto hace que tu HTML sea más rápido de escribir y mantener.

## Contenedores (.container)

Casi todo en Bootstrap empieza dentro de un container.
Sirve para centrar el contenido y definir el ancho máximo del sitio.

Tipos:

**.container →** ancho fijo que cambia según el tamaño de pantalla

**.container-fluid →** siempre ocupa el 100% del ancho

Ejemplo:

    <div class="container">
    <h1>Mi sitio con Bootstrap</h1>
    </div>

### Otras clases útiles

| Tipo       | Ejemplo                                               | Qué hace                             |
| ---------- | ----------------------------------------------------- | ------------------------------------ |
| Colores    | `.text-primary`, `.bg-danger`                         | Cambia color de texto o fondo        |
| Espaciado  | `.m-3`, `.p-2`                                        | `m`=margin, `p`=padding, números 0–5 |
| Alineación | `.text-center`, `.d-flex`, `.justify-content-between` | Centra o distribuye elementos        |
| Tamaños    | `.w-50`, `.h-100`                                     | Define ancho y alto relativos        |

Ejemplo:

    <div class="bg-light p-3 text-center">
    Caja centrada con fondo gris
    </div>

## Sistema de grillas (Grid System)

Bootstrap usa un sistema de 12 columnas para ordenar los elementos.
Todo empieza con una fila (.row) y dentro se colocan las columnas (.col).

Ejemplo básico:

    <div class="container">
    <div class="row">
        <div class="col">Columna 1</div>
        <div class="col">Columna 2</div>
        <div class="col">Columna 3</div>
    </div>
    </div>

También se pueden ajustar según el tamaño de pantalla:

    <div class="col-12 col-md-6 col-lg-4">Columna adaptable</div>

Esto permite crear estructuras que se adaptan automáticamente a celulares, tablets y computadoras.

## Componentes

Bootstrap incluye componentes listos para usar, que ya vienen con estilo y comportamiento integrado.
Solo hay que copiar su estructura y aplicar las clases correspondientes.

Ejemplos de componentes:

- Botones (.btn, .btn-primary)
- Cards (tarjetas con imagen y texto)
- Navbars (menús de navegación)
- Formularios (.form-control, .form-label)
- Modales (ventanas emergentes)
- Alertas (.alert, .alert-warning)

📘 Todos están documentados con ejemplos en getbootstrap.com/docs

## Breakpoints (diseño responsive)

Bootstrap adapta el diseño automáticamente usando breakpoints, o sea, “puntos de corte” de pantalla.

| Tamaño    | Clase base    | Dispositivo aproximado |
| --------- | ------------- | ---------------------- |
| `col-`    | Extra pequeño | Celulares              |
| `col-sm-` | Pequeño       | Tablets vertical       |
| `col-md-` | Mediano       | Tablets horizontales   |
| `col-lg-` | Grande        | Laptops                |
| `col-xl-` | Extra grande  | Monitores grandes      |


Ejemplo:

    <div class="col-12 col-md-6 col-lg-3">Se adapta a cada tamaño</div>
