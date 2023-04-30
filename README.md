# RESTfulApi-SpringBoot-Inventario
RESTful Api de gestion de inventario de productos.
- Lista productos, categorias y proveedores registrados.
- Mediante UI permite agregar, editar y eliminar informacion de las tablas. 
- Usa MySQL como gestor de base de datos

## Requerimientos

- Java JDK 17
- Spring Boot 3.0.5
- Maven 3.1.1, definida en .mvn/wrapper/maven-wrapper.properties
- MySQL 8.0.21

## Levantar proyecto:
### 1. Modificar las propiedades de la aplicacion
En el archivo ```src/main/resources/application.properties``` modificar las siguientes propiedades:
```sh 
    spring.datasource.url=jdbc:mysql://localhost:3306/bd_inventario
    spring.datasource.username=test
    spring.datasource.password=1234
    spring.jpa.hibernate.ddl-auto=none
    server.port=8091
```
1.1.  Crear la base de datos, con el siguiente script SQL:
```sh
create database bd_inventario;
```
1.2.  En "__username__" y "__password__" colocar sus credenciales de MySQL.

1.3.  Cambiar el valor a spring.jpa.hibernate.ddl-auto=__update__

1.4.  Cambiar el puerto al que deseen, siempre y cuando no este usado por otro servicio.

## 2. Correr la aplicacion
Correr la clase princial __InventarioApplication__ que contiene el metodo __main__

Abrir cualquier navegador e ingresar a la url: __localhost:8091/home__

# Screenshots
