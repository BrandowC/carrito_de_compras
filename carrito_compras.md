# Proyecto de Sistema de Carrito de Compras

## Introducción
Este proyecto implementa un sistema de carrito de compras en el cual los usuarios pueden registrarse, iniciar sesión, navegar por un catálogo de productos, agregar productos al carrito, gestionar el carrito y generar una factura al confirmar la compra.

## Requerimientos Funcionales
1. **RF01: Registro e Inicio de Sesión**
   - El sistema permite a los usuarios registrarse e iniciar sesión para acceder a sus carritos de compras.

2. **RF02: Catálogo de Productos**
   - Los usuarios pueden buscar y visualizar productos con nombre, descripción, precio y cantidad en stock.

3. **RF03: Agregar Productos al Carrito**
   - El sistema permite agregar productos al carrito, especificando la cantidad deseada.

4. **RF04: Gestión del Carrito de Compras**
   - Los usuarios pueden visualizar el contenido de su carrito, modificar cantidades o eliminar productos.

5. **RF05: Generación de Factura**
   - Al confirmar la compra, el sistema genera una factura con el detalle de productos, cantidades, precios e impuestos.

## Pasos para la Implementación

### 1. Configuración del Entorno
- **Backend**: Spring Boot
- **Frontend**: Angular
- **Base de Datos**: MySQL (usando XAMPP)

### 2. Registro e Inicio de Sesión
- Crear el modelo de usuario, la tabla correspondiente en la base de datos, y usar Spring Security para manejar la autenticación.

### 3. Catálogo de Productos
- Crear un modelo `Producto` que incluya los atributos `nombre`, `descripcion`, `precio`, `stock`.
- Implementar un endpoint en Spring Boot para mostrar los productos, y una interfaz en Angular para que los usuarios los puedan visualizar.

### 4. Agregar Productos al Carrito
- Crear el modelo de `Carrito` y permitir que los usuarios agreguen productos desde el catálogo.
  
### 5. Gestión del Carrito de Compras
- Proporcionar vistas en Angular para ver los productos del carrito y permitir modificaciones o eliminación de productos.

### 6. Generación de Factura
- Implementar un servicio que genere una factura una vez que los productos en el carrito sean confirmados para compra.

## Prototipo de la Interfaz de Usuario

### Pantalla de Registro e Inicio de Sesión
![Registro](USUARIO.drawio.png)

### Catálogo de Productos
![Catálogo](productos.drawio.png)

### Carrito de Compras
![Carrito](compras.drawio.png)

### Generación de Factura
![Factura](facturas.drawio.png)

### Relación entre los diagramas:
- El **Usuario** tiene un **compras**.
- El **compras** contiene múltiples **Productos**.
- La **Factura** contiene los **Productos** comprados y es generada a partir del **comopras**.

## Herramientas Utilizadas
- **Backend**: Spring Boot
- **Frontend**: Angular
- **Base de Datos**: MySQL
- **Herramientas para diagramas**: Lucidchart / Draw.io
