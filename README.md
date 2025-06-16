# GAMJE VISUAL - Plataforma Educativa Modular (Frontend)

**Gamje Visual** es la interfaz gráfica de la plataforma educativa GAMJE, una solución modular basada en arquitectura de microservicios que busca transformar la experiencia de aprendizaje digital.

Este repositorio contiene las vistas HTML/CSS/JS organizadas por perfiles de usuario, simulando la interacción directa con los servicios RESTful del backend implementado con Spring Boot. La interfaz está pensada para ser simple, funcional y escalable, apta para estudiantes, profesores, administradores y visitantes.

## 🌐 URL de despliegue (GitHub Pages)

> Asegúrate de haber configurado correctamente GitHub Pages en la rama correspondiente para visualizarlo en línea.  
> Por ejemplo: `https://<usuario>.github.io/gamje-visual/estudiante/home-estudiante`

---

## 🧩 Funcionalidades del sistema (Frontend)

### 🔑 Inicio de Sesión
- `/login` — Página principal de login
- `/login/crear-cuenta` — Registro de nuevos usuarios
- `/login/encuentra-cuenta` — Recuperación de cuenta por correo

### 🎓 Perfil Estudiante
- `/estudiante/home-estudiante` — Vista principal del alumno
- `/estudiante/explorar-cursos-estudiante` — Navegación del catálogo de cursos
- `/estudiante/cursos-estudiante` — Visualización de cursos inscritos
- `/estudiante/foro-curso-estudiante` — Participación en foros de clase
- `/estudiante/videochat-estudiante` — Acceso a videollamadas en línea
- `/estudiante/pago-mensualidad-estudiante` — Formulario de pago mensual

### 👨‍🏫 Perfil Profesor
- `/profesor/home-profesor` — Panel principal del docente
- `/profesor/cursos-profesor` — Gestión de cursos impartidos
- `/profesor/cursos-detalle-profesor` — Detalle y contenidos del curso
- `/profesor/foro-curso-profesor` — Moderación del foro
- `/profesor/chats-videollamada-profesor` — Acceso a chats y videollamadas

### 🛠 Perfil Administrador
- `/admin/Ingresos-admin` — Control de ingresos mensuales
- `/admin/centro-ayuda-admin` — Gestión de solicitudes de ayuda
- `/admin/estado-microservicios-admin` — Estado actual de los microservicios
- `/admin/gestion-usuarios-admin` — Panel de administración de usuarios
- `/admin/roles-usuarios-admin` — Asignación de roles y permisos
- `/admin/settings-admin` — Configuraciones generales

### 📊 Vistas Generales
- `/general/dashboard-analytics-graficos` — Analítica visual de la plataforma
- `/general/manejo-cursos` — Herramientas comunes para gestión de cursos
- `/general/reporte-problemas` — Envío de reportes de errores

---

## 🔧 Tecnologías Utilizadas

Frontend:
- HTML5 / CSS3
- JavaScript Vanilla + Fetch API
- Bootstrap 5 (opcional)
- Sublime Text / Visual Studio Code

Backend (referencial):
- Java 24 con Spring Boot
- API REST + Swagger UI
- WebClient para microservicios
- Bases de Datos: MySQL / PostgreSQL

Control de versiones:
- Git + GitHub

---

## 📌 Consideraciones

- Este proyecto es una **simulación funcional** orientada al consumo de microservicios ya implementados en el backend de GAMJE.
- Las vistas fueron organizadas para representar distintos perfiles de usuario, y las rutas siguen la lógica de una posible arquitectura en producción.
- Las pruebas funcionales se realizaron con Thunder Client y Postman para validar la comunicación con los endpoints REST.

---

## 🚀 ¿Cómo contribuir?

1. Clona el repositorio:
   ```bash
   git clone https://github.com/GersebO/gamje-visual.git

