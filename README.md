

## 1. Contexto papu

He cambiado la aplicacion original de tareas por una lista de la compra. lo elegi porque es facil :p y se parece a la app base un poco 

## 2. Estructura de la base de datos

La aplicacion usa SQLite y guarda los datos en el archivo `tareas.db`.

Tabla: `Tareas`

| Columna Para que sirve |
| ---  |
| Id // Identifica cada producto /
| Nombre  / Nombre del producto //
| Cantidad // Cantidad que hay que comprar 
| Comprado //   Indica si ya esta comprado 

## 3. URLs de la aplicacion

| URL de la app: // Que hacen :
| `/` | Muestra la lista completa de productos |
| `/?filtro=todos` | Muestra todos los productos |
| `/?filtro=pendientes` | Muestra solo los productos pendientes |
| `/?filtro=comprados` | Muestra solo los productos comprados |
| `/Tareas/Crear` | Abre el formulario para crear un producto |
| `/Tareas/Editar/{id}` | Abre el formulario para editar un producto existente |
| `/Tareas/Completar/{id}` | Marca un producto como comprado |
| `/Tareas/Eliminar/{id}` | Elimina un producto.

## 4. Cambios realizados respecto al codigo base

- Se cambio el contexto de tareas a lista de la compra. 
- El modelo ahora son productos con `Nombre`, `Cantidad` y `Comprado`.
- Se añadio el campo extra `Cantidad`para especificar lo de los productos.
- Se actualizo la base de datos.
- Se actualizo la vista principal para mostrar el nombre, la cantidad y el estado (comprao o en la lista)
- Se añadio la opcion de editar productos.
- El formulario de editar aparece relleno con los datos actuales.
- Se añadieron limites
  - El nombre no puede estar vacio.
  - El nombre debe tener mas de 2 caracteres.
  - La cantidad debe ser como minimo 1.
- Si  falla, aparece un mensaje de error en la misma pagina.
- Se añadio filtrado por todos, pendientes y comprados.
- Se cambio el CSS a un estilo blanco y negro con fondo de cuadrados y caritas `:)` porque mola.

## 5. Capturas de pantalla :d

### Vista principal

<img width="1919" height="963" alt="Captura de pantalla 2026-05-20 170436" src="https://github.com/user-attachments/assets/01bab438-4a8a-4087-a400-1c0f3ed0ca96" />

### Crear producto
<img width="1919" height="957" alt="Captura de pantalla 2026-05-20 170456" src="https://github.com/user-attachments/assets/b248ddab-4b11-481a-9066-b5f7632d4df2" />

### Editar producto
<img width="776" height="246" alt="Captura de pantalla 2026-05-20 170523" src="https://github.com/user-attachments/assets/6bdfd504-4c25-4360-9b3a-ba55bdc3ca5d" />
<img width="1917" height="963" alt="Captura de pantalla 2026-05-20 170448" src="https://github.com/user-attachments/assets/bba6d1b3-b5a0-4134-a303-b9de746948f4" />




### Filtro de comprados

<img width="776" height="246" alt="Captura de pantalla 2026-05-20 170523" src="https://github.com/user-attachments/assets/c3a59bcd-d554-408e-a21c-35e337216f6d" />


### Error 
<img width="1917" height="956" alt="Captura de pantalla 2026-05-20 170425" src="https://github.com/user-attachments/assets/5e9052c7-95bf-4457-990b-643972d7cc6b" />


tuerelocomenol
