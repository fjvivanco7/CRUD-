# CRUD en Java

Este proyecto implementa un sistema **CRUD (Create, Read, Update, Delete)** desarrollado en **Java**.  
Su objetivo es demostrar la gestión básica de datos en una base de datos relacional utilizando consultas SQL.

## 📌 Descripción

El sistema permite realizar operaciones sobre una tabla de base de datos, manejando registros de manera eficiente y sencilla.  
Incluye las siguientes funcionalidades:

- **Crear**: Insertar nuevos registros.
- **Leer**: Listar y consultar registros existentes.
- **Actualizar**: Modificar registros existentes.
- **Eliminar**: Borrar registros de forma permanente.

Este CRUD fue desarrollado como práctica académica y puede servir como base para proyectos más avanzados.

## 🛠️ Tecnologías utilizadas

- **Lenguaje**: Java 17 (puede funcionar con versiones anteriores compatibles)
- **Base de datos**: MySQL
- **Conector**: JDBC (Java Database Connectivity)
- **IDE recomendado**: IntelliJ IDEA / Eclipse / NetBeans

## 📂 Estructura del proyecto

📦 crud-java
┣ 📂 src
┃ ┣ 📂 model # Clases del modelo (entidades)
┃ ┣ 📂 dao # Data Access Object (métodos CRUD)
┃ ┣ 📂 util # Configuración de conexión a la BD
┃ ┗ 📂 main # Clase principal con menú y lógica
┣ 📄 README.md
┣ 📄 pom.xml # (Si se usa Maven)


## ⚙️ Requisitos previos

Antes de ejecutar el proyecto, asegúrate de tener instalado:

- **Java JDK 17** o superior  
- **MySQL Server** y **MySQL Workbench**  
- **Driver JDBC para MySQL** (`mysql-connector-java-x.x.x.jar`)  

Configura una base de datos con la siguiente estructura de ejemplo:

```sql
CREATE DATABASE crud_db;

USE crud_db;

CREATE TABLE usuarios (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nombre VARCHAR(100) NOT NULL,
    correo VARCHAR(100) NOT NULL,
    edad INT NOT NULL
);

🚀 Ejecución

Clona este repositorio:
git clone https://github.com/tuusuario/crud-java.git

Importa el proyecto en tu IDE.

Configura la conexión a la base de datos en la clase Conexion.java:

private static final String URL = "jdbc:mysql://localhost:3306/crud_db";
private static final String USER = "root";
private static final String PASSWORD = "tu_contraseña";

Ejecuta la clase Main.java.

Usa el menú en consola para interactuar con las operaciones CRUD.
===== MENÚ CRUD =====
1. Crear usuario
2. Listar usuarios
3. Actualizar usuario
4. Eliminar usuario
5. Salir
Seleccione una opción:
📌 Funcionalidades futuras

Implementación de interfaz gráfica con Java Swing / JavaFX.

Migración a un entorno Spring Boot + JPA.

Integración con API REST.

👨‍💻 Autor

Fernando Vivanco

Proyecto académico de prácticas en programación con Java.
