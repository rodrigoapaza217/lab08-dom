# Bitacora de JavaScript interactivo

Laboratorio 08: JavaScript Interactivo - DOM, Eventos y Objetos.

Navegador usado: ( Chrome )

##	Ejercicio	2:	Seleccionar y modificar el DOM

| Instruccion | Que cambio en la pantalla | Se mantiene al recargar (Si/No) |
|---|---|---|
| textContent desde la consola | Cambió el título principal a "Hola desde la consola"| No|
| textContent desde app.js | Cambió el título principal a "Hola TECSUP"| Si|
| style.color | Cambió el color del título a azul| Si|
| classList.add | Le aplicó la clase de estilo destacado (fondo amarillo) al párrafo| Si|
| createElement + appendChild | Agregó un nuevo ítem "JavaScript" a la lista de elementos| Si|


##	Ejercicio	3:	Evento click

| Tipo de evento | Que accion lo dispara | Cuanto suma por accion |
|---|---|---|
| click | hace click izquierdo normal sobre el boton| +1 |
| dblclick | hacer doble click rapidamente para que lo accione| +1 |
| mouseover | Al pasar el puntero sobre el boton lo acciona sin dar click| +1 |

##	Ejercicio	4:	Eventos input y submit

| Prueba | Qué pasó en la pantalla | Se recargó la página (Sí/No) |
|---|---|---|
| Escribir en el campo nombre | El saludo "Hola, ..." se fue actualizando letra por letra en tiempo real. | No |
|Enviar sin preventDefault | El mensaje de envío apareció un instante pero desapareció de inmediato. | Sí |
| Enviar con preventDefault, correo sin @ | Mostró el mensaje "Correo no valido: falta @" en texto rojo. | No |
| Enviar con preventDefault, correo con @ | Mostró el mensaje "Enviado: correo@ejemplo.com" correctamente. | No |

##	Ejercicio	5:	Clases y objetos

| Objeto | nombre | precio | descripcion() | conDescuento(0.25) |
|---|---|---|---|---|
| `laptop` | Laptop | 2500 | Laptop - S/ 2500.00 | 1875.00 |
| `mouse` | Mouse | 45 | Mouse - S/ 45.00 | 33.75 |
| `teclado` | Teclado | 120 | Teclado - S/ 120.00 | 90.00 |
| `monitor` | Monitor | 680 | Monitor - S/ 680.00 | 510.00 |

##	Ejercicio	6:	DOM, eventos y objetos juntos

| Prueba | Total que muestra la página | Correcto (Sí/No) |
|---|---|---|
| Cuaderno 12.50 | 12.50 | Sí |
| + Lapicero 3.20 | 15.70 | Sí |
| + Mochila 89.90 | 105.60 | Sí |
| Sin Number() | Error en consola (`this.precio.toFixed is not a function`) | No |

| Pieza | Línea de tu código donde aparece | Para qué sirve |
|---|---|---|
| DOM | `document.querySelector("#carrito")` | Selecciona elementos del HTML para leer sus valores o modificarlos dinámicamente. |
| Evento | `formProducto.addEventListener("submit", ...)` | Escucha la acción de envío del formulario para ejecutar la función sin recargar la página. |
| Objeto | `new Producto(...)` / `new Carrito()` | Crea e instancia la estructura que organiza los datos del producto y gestiona la lista de compras. |