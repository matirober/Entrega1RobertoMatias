# Entrega1RobertoMatias
Entrega numero 1 del curso de sql coderhouse


Base de datos de cadena de Supermercados

En esta base de datos podras ver la relacion ente tablas y como se comportan dentro de la base misma, de cualquier supermercado de la cadena

Las tablas que lo componen son:
Cliente:
PK idCliente iNT NotNull
PK Consumo Float NotNull
NombreCliente Int
MailCliente varchar(50)
DireccionCliente varchar(45)
FK Ventas_idVentas INT NotNull

Productos:
PK idProducto varchar(50) NotNull
PK nombreProducto varchar(45) NotNull
PK precioProductoVenta Float

Proveedores:
PK idProveedores varchar(50) NotNull
PK precioProductoCompra Float NotNull
nombreProveedor varchar(50)

Ventas:
PK idVentas Int NotNull Autoincremental
FK Producto_idProducto NotNull Int
FK Producto_nombreProducto NotNull varchar(45)
FK Producto_precioProducto NotNull varchar(45)
FK Empleados_idEmpleado Int NotNull
FK Sucursal_idSucursal Int NotNull

Compras:
PK idCompras Int NotNull Autoincremental
FK Producto_idProducto NotNull Int
FK Producto_nombreProducto NotNull varchar(45)
FK Proveedores_idProveedores NotNull Int
FK Proveedores_precioProveedores NotNull Float

Descuentos:
PK idDescuentos Int NotNull Autoincremental
FK Producto_idProducto NotNull varchar(50)
FK Producto_nombreProducto NotNull varchar(45)
FK Producto_precioProductoVenta NotNull Float

Sucursal:
PK idSucursal Int NotNull Autoincremental
FK Empleados_idEmpleados Int NotNull
FK Compras_idCompras Int NotNull
nombreSucursal varchar (50)

Ganancias:
PK idGanancias Int NotNull Autoincremental

Empleados:
PK idEmpleados Int NotNull Autoincremental
nombreEmpleado Varchar(45)
