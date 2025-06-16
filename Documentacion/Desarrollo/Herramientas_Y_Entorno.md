# 🛠️ Entorno de Desarrollo y Herramientas - Proyecto GAMJE

Este documento describe el conjunto de herramientas, frameworks, tecnologías y entornos utilizados en el desarrollo del proyecto **GAMJE**, una plataforma educativa modular basada en microservicios y frontend desacoplado.

## 🧰 Herramientas Utilizadas

### ⚙️ Backend - Microservicios
- **Java 24**  
  Lenguaje principal para el desarrollo de microservicios.
- **Spring Boot 3.4.5**  
  Framework para la creación de aplicaciones Java modernas y desacopladas.
- **Spring Web**  
  Para la construcción de controladores RESTful.
- **Spring Data JPA**  
  Para la conexión con la base de datos y manejo de entidades.
- **Lombok**  
  Para simplificar el código eliminando la necesidad de escribir getters/setters manuales.
- **WebClient**  
  Para la comunicación entre microservicios (asincrónica y desacoplada).

### 🧪 Testing y Documentación
- **Postman**  
  Herramienta para testeo de endpoints.
- **Swagger/OpenAPI**  
  Documentación interactiva de los endpoints REST. Se usó `springdoc-openapi` para autogenerar la documentación.
- **JUnit**  
  Framework para pruebas unitarias (opcional en este proyecto).

### 🗄️ Base de Datos
- **MySQL**  
  Sistema de gestión de base de datos relacional (local y en producción).
- **Neon.tech (PostgreSQL)**  
  Se utilizó en algunas pruebas para despliegue cloud, especialmente con Python.

### 🔌 Dependencias (Maven)
El proyecto usa Maven como gestor de dependencias. Las principales:
```xml
<dependencies>
  <dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
  </dependency>
  <dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-jpa</artifactId>
  </dependency>
  <dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-validation</artifactId>
  </dependency>
  <dependency>
    <groupId>org.springdoc</groupId>
    <artifactId>springdoc-openapi-starter-webmvc-ui</artifactId>
    <version>2.0.4</version>
  </dependency>
  <dependency>
    <groupId>org.projectlombok</groupId>
    <artifactId>lombok</artifactId>
    <optional>true</optional>
  </dependency>
</dependencies>
```

## 🖥️ Frontend (GAMJE Visual)
- **HTML/CSS/JavaScript**  
  Lenguajes estándar para construir las vistas del usuario.
- **GitHub Pages**  
  Para el despliegue del frontend estático.
- **Figma / Canva**  
  Herramientas de diseño de interfaz para prototipado rápido y mockups.

## 🔄 Control de Versiones y Repositorio
- **Git**  
  Sistema de control de versiones distribuido.
- **GitHub**  
  Plataforma para alojar el código y documentación.  
  Repositorio: [https://github.com/GersebO/gamje-microservicios](https://github.com/GersebO/gamje-microservicios)

## 🧪 Entorno de Desarrollo Local

- **IDE Recomendado:** Visual Studio Code o IntelliJ IDEA
- **Java SDK:** Java 24
- **MySQL Server:** 8.0+
- **Herramientas CLI:** Maven (`mvn`), Git

## 🚀 Despliegue y Testing

- **Postman** para probar manualmente los endpoints REST.
- **Swagger UI** disponible en cada microservicio en la ruta `/swagger-ui.html`.

## 📦 Organización del Proyecto

Cada microservicio se encuentra estructurado de manera independiente:

```
gamje-microservicios/
│
├── usuarios/
├── cursos/
├── inscripciones/
├── pagos/
├── evaluacion/
├── gateway/
└── README.md
```

## 🌐 Otros Servicios

- **API Gateway**  
  Usado como puerta de entrada unificada para todos los microservicios.
- **DTO y Validaciones**  
  Se implementaron DTOs para abstraer la lógica de entrada/salida y validaciones con `@Valid`.

## 📌 Requisitos Previos

Asegúrate de tener instalado:

- Java 24
- Maven 3.8+
- MySQL Server
- IDE como IntelliJ o VSCode
- Git
- Navegador web (para usar Swagger y GitHub Pages)
