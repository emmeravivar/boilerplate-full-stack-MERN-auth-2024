# full-stack-MERN-auth-2024

Proyecto full stack MERN para autenticación de usuarios.

## Propósito
Sistema base para registro, login, confirmación de cuenta, recuperación de contraseña y gestión de perfiles de usuario usando el stack MERN (MongoDB, Express, React, Node.js).

## Backend (server)
- **Librerías principales:**
  - express, mongoose, dotenv, cors, bcrypt, jsonwebtoken, nodemailer
- **Endpoints principales:**
  - `POST /api/user/create-user` — Crear nuevo usuario
  - `POST /api/user/login` — Login de usuario
  - `GET /api/user/confirm-account/:token` — Confirmar cuenta por token
  - `POST /api/user/reset-password` — Solicitar recuperación de contraseña
  - `GET /api/user/reset-password/:token` — Verificar token de recuperación
  - `POST /api/user/reset-password/:token` — Cambiar contraseña
  - `GET /api/user/profile` — Obtener perfil del usuario autenticado (privado)
  - `GET /api/user/user-profile` — Obtener perfil de otro usuario (privado)

## Frontend (client)
- **Librerías principales:**
  - react, react-dom, react-router-dom, axios, tailwindcss, vite
- **Funcionalidades:**
  - Registro y login de usuarios
  - Confirmación de cuenta y recuperación de contraseña
  - Acceso a dashboard privado tras autenticación
  - Visualización y edición de perfil de usuario
  - Navegación protegida por rutas y layouts

---

Configura el archivo `.env` en el backend con las variables necesarias para la conexión a MongoDB y URLs permitidas por CORS.