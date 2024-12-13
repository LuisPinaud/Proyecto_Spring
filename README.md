# 📚 Mantenimiento de Libros con Spring Framework

Este proyecto es un sistema de mantenimiento de libros desarrollado con **Spring Framework**, utilizando una arquitectura basada en capas. El objetivo principal del sistema es gestionar información de libros en una base de datos, permitiendo realizar operaciones CRUD (Crear, Leer, Actualizar y Eliminar).

## 🚀 Funcionalidades

- Gestión de información de libros.
- Operaciones CRUD completas sobre la base de datos.
- Separación clara de responsabilidades mediante una arquitectura en capas.
- Utilización de utilitarios para tareas comunes.

## 🛠️ Tecnologías Utilizadas

- **Java 17**: Lenguaje de programación principal.
- **Spring Framework**: Base para el desarrollo del proyecto.
- **Spring Data JPA**: Gestión de las entidades y repositorios.
- **Spring MVC**: Controladores y manejo de solicitudes HTTP.
- **Spring Boot**: Configuración automática del proyecto.
- **MySQL**: Base de datos utilizada.
- **Hibernate**: Implementación de JPA para la persistencia de datos.
- **Maven**: Gestión de dependencias y construcción del proyecto.

## 📂 Arquitectura del Proyecto

El proyecto sigue una estructura en capas para garantizar la separación de responsabilidades:

### Model:
- Contiene las entidades generadas automáticamente desde la base de datos.
- Cada clase de entidad mapea una tabla de la base de datos.

### Repository:
- Interfaces que extienden `JpaRepository` para interactuar con la base de datos.

### Service:
- Define las reglas de negocio.
  - **Impl**: Implementa los métodos de la capa `Service`.

### Controller:
- Maneja las solicitudes HTTP y las respuestas hacia el cliente.

### Utils:
- Contiene clases utilitarias, como validadores o formateadores.
