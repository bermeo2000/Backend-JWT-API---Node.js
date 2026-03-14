
# Backend JWT API - Node.js

📌 **Descripción**

Este proyecto es una API REST desarrollada con Node.js y Express que implementa autenticación mediante JSON Web Token (JWT). Permite registrar usuarios, iniciar sesión y gestionar usuarios utilizando una base de datos MySQL mediante Sequelize.

El proyecto fue desarrollado como parte de prácticas del módulo de Desarrollo Web y Aplicaciones.

🚀 **Tecnologías utilizadas**

- Node.js
- Express
- MySQL
- Sequelize ORM
- JWT (jsonwebtoken)
- bcryptjs
- dotenv
- CORS

📂 **Estructura del proyecto**

```
backend-jwt
│
├── src
│   ├── controllers
│   ├── models
│   ├── routes
│   ├── middlewares
│   ├── app.js
│   └── server.js
│
├── node_modules
├── .env
├── package.json
└── README.md
```

⚙️ **Instalación del proyecto**

1️⃣ **Clonar el repositorio**

```bash
git clone https://github.com/TU_USUARIO/backend-jwt.git
```

2️⃣ **Entrar al proyecto**

```bash
cd backend-jwt
```

3️⃣ **Instalar dependencias**

```bash
npm install
```

🗄️ **Configuración de la base de datos**

Crear una base de datos en MySQL:

```sql
CREATE DATABASE daw_espam;
```

🔑 **Configuración del archivo .env**

Crear un archivo `.env` en la raíz del proyecto:

```
PORT=5000

DB_HOST=localhost
DB_PORT=3306
DB_NAME=daw_espam
DB_USER=root
DB_PASSWORD=
DB_DIALECT=mysql

JWT_SECRET=clave_super_secreta
JWT_EXPIRES_IN=1h
```

▶️ **Ejecutar el proyecto**

Modo desarrollo:

```bash
npm run dev
```

Modo producción:

```bash
npm start
```

El servidor se ejecutará en:

```
http://localhost:5000
```

📡 **Endpoints principales**

**Obtener estado de la API**

`GET /`

**Registrar usuario**

`POST /api/v1/auth/register`

Ejemplo:

```json
{
  "nombres": "Luis Macias",
  "email": "luis@maestria.com",
  "password": "Clave.2026",
  "rol": "admin"
}
```

**Iniciar sesión**

`POST /api/v1/auth/login`

Ejemplo:

```json
{
  "email": "luis@maestria.com",
  "password": "Clave.2026"
}
```

**Obtener usuarios**

`GET /api/v1/users`

🧪 **Pruebas de la API**

Las pruebas se pueden realizar usando:

- REST Client en VS Code
- Postman
- Insomnia

👨‍💻 **Autor**

Luis Antonio Macías Bermeo

Proyecto académico de desarrollo de backend con autenticación JWT.

📄 **Licencia**

Este proyecto se distribuye bajo licencia MIT.
