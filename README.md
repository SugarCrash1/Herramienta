# Herramienta

Aplicación full-stack con backend en Spring Boot y dos frontends en React/Vite.

## Requisitos

- Docker
- Docker Compose

## Ejecutar con Docker Compose

Desde la raíz del proyecto:

```bash
docker compose up --build -d
```

Esto levanta:

- Backend en http://localhost:8081
- Frontend admin en http://localhost:5173
- Frontend tickets en http://localhost:5174
- PostgreSQL en localhost:5433

## Verificar que todo funcione

```bash
curl http://localhost:8081/usuarios
curl -I http://localhost:5173
curl -I http://localhost:5174
```

## Detener los servicios

```bash
docker compose down
```

## Detener y borrar datos de la base de datos

```bash
docker compose down -v
```

## Credenciales por defecto

La aplicación inicializa un usuario administrador con:

- Email: admin@gmail.com
- Contraseña: admin123
