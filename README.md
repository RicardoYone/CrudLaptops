# CRUD Laptops

Este repositorio contiene dos proyectos independientes:

- **backend**: API RESTful desarrollada en Laravel (PHP).
- **vue-project**: Aplicación frontend desarrollada en Vue.js.

## Estructura del repositorio

```
├── backend/      # API en Laravel
├── vue-project/  # Frontend en Vue.js
└── README.md     # Este archivo
```

## Tecnologías usadas

- **Backend:** Laravel, PHP, PosgresSQL
- **Frontend:** Vue.js, Vite

## Instrucciones para levantar el sistema

### 1. Clonar ambos proyectos

Puedes clonar este repositorio y luego subir cada carpeta (`backend` y `vue-project`) a GitHub como repositorios independientes.

### 2. Levantar el backend (Laravel)

1. Ir a la carpeta `backend`:
   ```bash
   cd backend
   ```
2. Instalar dependencias:
   ```bash
   composer install
   npm install
   ```
3. Copiar el archivo de entorno:
   ```bash
   cp .env.example .env
   ```
4. Configurar la base de datos (por defecto usa PosgresSQL):
   - Verifica que `DB_CONNECTION=pgsql` en `.env`.
   - El archivo `database/database.sqlite` ya está creado.
5. Ejecutar migraciones y seeders:
   ```bash
   php artisan migrate --seed
   ```
6. Levantar el servidor:
   ```bash
   php artisan serve
   ```
   El backend estará disponible en `http://localhost:8000`

### 3. Levantar el frontend (Vue.js)

1. Ir a la carpeta `vue-project`:
   ```bash
   cd vue-project
   ```
2. Instalar dependencias:
   ```bash
   npm install
   ```
3. Levantar el servidor de desarrollo:
   ```bash
   npm run dev
   ```
   El frontend estará disponible en `http://localhost:5173`

## Buenas prácticas de Git

- Usa ramas para nuevas funcionalidades o correcciones.
- Escribe mensajes de commit claros y descriptivos.
- Haz uso de `.gitignore` para evitar subir archivos sensibles o innecesarios.
- Realiza `pull` y `push` frecuentemente para mantener el repositorio actualizado.

---
