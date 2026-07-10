# Colegio SaaS

Sistema de gestión escolar desarrollado con Laravel para administrar de manera integral los procesos académicos y administrativos de una institución educativa.

## Descripción general

Este proyecto ofrece una solución moderna para la gestión escolar, permitiendo centralizar operaciones clave como:

- Gestión de estudiantes, docentes, cursos y materias
- Matrículas, promociones y seguimientos académicos
- Registro de asistencia y control de calificaciones
- Asignaciones, tareas y entregas estudiantiles
- Comunicación interna, anuncios y mensajes
- Gestión de pagos, deudores y estados financieros básicos
- Control de biblioteca y préstamos de materiales
- Generación de reportes y documentos escolares
- Configuración del sistema y trazabilidad mediante bitácora de auditoría

## Tecnologías utilizadas

- PHP 8.2+
- Laravel 11
- Composer
- MySQL / MariaDB
- Blade Templates
- DomPDF para la generación de documentos PDF

## Requisitos previos

Antes de instalar el proyecto, asegúrate de contar con:

- PHP 8.2 o superior
- Composer
- MySQL o MariaDB
- Un servidor local o acceso a Laravel Serve

## Instalación

1. Clona el repositorio:

```bash
git clone <url-del-repositorio>
cd saas_colegio
```

2. Instala las dependencias del proyecto:

```bash
composer install
```

3. Copia el archivo de entorno:

```bash
copy .env.example .env
```

4. Configura la conexión a la base de datos en el archivo `.env`:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=saas_colegio
DB_USERNAME=root
DB_PASSWORD=
```

5. Genera la clave de la aplicación:

```bash
php artisan key:generate
```

6. Ejecuta las migraciones y seeders si están disponibles:

```bash
php artisan migrate
php artisan db:seed
```

7. Inicia el servidor de desarrollo:

```bash
php artisan serve
```

Abre tu navegador en:

```text
http://localhost:8000
```

## Uso del sistema

La plataforma está diseñada para distintos roles de usuario, como:

- Administrador
- Secretaría
- Docente
- Superadministrador

La autenticación está disponible en las rutas `/login` y `/registro`.

## Estructura del proyecto

- `app/`: lógica principal de la aplicación, controladores, modelos y servicios
- `config/`: configuraciones del sistema
- `public/`: archivos públicos y punto de entrada web
- `resources/views/`: vistas Blade
- `routes/`: definiciones de rutas del sistema
- `storage/`: archivos generados por la aplicación

## Contribución

Si deseas colaborar con el proyecto:

1. Haz un fork del repositorio
2. Crea una rama para tu cambio
3. Desarrolla tus modificaciones
4. Envía un pull request

## Licencia

Este proyecto está bajo la licencia MIT.

---

<div align="center">
  <strong>Elaborado por:</strong><br>
  <em>Huanca Flores Juan Pablo</em><br>
  <em>Rojas Rodriguez Wilmer</em><br>
  <strong>Analista de Sistemas 2026</strong>
</div>
