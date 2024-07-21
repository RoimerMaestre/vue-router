![alt](./src/assets/img/Captura%20de%20pantalla%202024-07-20%20155537.png)

# Proyecto Vue.js - Tienda de Productos

Este proyecto es una aplicación web simple desarrollada con Vue.js que muestra una tienda de productos. Incluye un menú de navegación, vistas para productos y contacto, y utiliza lazy loading para cargar los componentes de manera eficiente.

## Características

<ul>
<li>Navegación entre páginas utilizando <router-link>.</li>
<li>Vistas para productos y contacto.</li>
<li>
Enlaces de redirección al inicio desde las vistas de Productos y Contacto.</li>
<li>Carga controlada de componentes (lazy loading).</li>
<li>Uso de props para pasar datos a los componentes.</li>
</ul>

## Componentes

### Navbar

El componente de navegación que permite la transición entre las diferentes vistas.

### Card

Componente que muestra la información de un producto utilizando props.

### Footer

Pie de página de la aplicación.

### MediosPago

Componente que muestra los medios de pago disponibles.

## Vistas

### HomeView

La vista principal que da la bienvenida a los usuarios y ofrece enlaces para ver productos y contactar.

### ProductoView

Vista que muestra información detallada de un producto. Recibe props para mostrar el nombre, descripción, precio y cantidad del producto.

### ContactoView

Vista que contiene un formulario de contacto y enlaces a redes sociales, así como un enlace para volver al inicio.

## Rutas

Las rutas están definidas en router/index.js y utilizan lazy loading para cargar los componentes de manera eficiente.
