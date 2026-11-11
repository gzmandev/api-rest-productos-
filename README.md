# API RESTful de Productos (PHP + PDO + MySQL)

**Curso:** Programación Web Básica  
**Tecnología:** PHP nativo, MySQL, PDO  
**Entorno:** XAMPP

## Descripción

API REST nativa en PHP para gestión de productos. Implementa GET, POST, PUT, DELETE con respuestas JSON, validaciones robustas, consultas preparadas y códigos HTTP apropiados.

## Instalación

1. Copia la carpeta en `C:\xampp\htdocs\`.
2. Inicia Apache y MySQL en XAMPP.
3. Importa `sql/evaluacion_api.sql` en phpMyAdmin.
4. Prueba: `http://localhost/api-rest-productos/api/productos.php`

## Endpoints

| Método | URL | Descripción |
|--------|-----|-------------|
| GET | `productos.php` | Lista productos |
| GET | `productos.php?id=3` | Producto por ID |
| POST | `productos.php` | Crea producto (JSON) |
| PUT | `productos.php?id=3` | Actualiza producto |
| DELETE | `productos.php?id=3` | Elimina producto |

## Estructura

```
api-rest-productos/
├── api/productos.php
├── config/conexion.php
├── sql/evaluacion_api.sql
└── evidencias/
```

## Notas

- Credenciales de DB en `config/conexion.php` (root / vacío, típico XAMPP).
- Para producción, mover credenciales a variables de entorno.