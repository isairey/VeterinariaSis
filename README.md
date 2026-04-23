# 🐾 API Veterinaria - Backend

API REST desarrollada en **C# con ASP.NET Core** para la gestión de una clínica veterinaria. Proporciona endpoints para administrar mascotas, dueños, citas médicas y el historial clínico.

---

## 🚀 Características

* 🐶 Gestión de mascotas (CRUD)
* 👤 Administración de dueños
* 📅 Control de citas veterinarias
* 🩺 Historial clínico
* 💊 Registro de tratamientos
* 🔐 Autenticación y autorización (JWT)
* 📡 API RESTful
* 📊 Estructura escalable y modular

---

## 🛠️ Tecnologías Utilizadas

* 💻 C#
* ⚙️ ASP.NET Core Web API
* 🗄️ SQL Server
* 🔗 Entity Framework Core
* 🔐 JWT Authentication
* 🧰 Visual Studio / VS Code

---

## 📦 Instalación

### 1️⃣ Clonar el repositorio

```bash id="x7n2k1"
git clone https://github.com/isairey/VeterinariaSis.git
cd VeterinariaSis
```

---

### 2️⃣ Restaurar dependencias

```bash id="g5y8k2"
dotnet restore
```

---

### 3️⃣ Configurar base de datos

Editar `appsettings.json`:

```json id="q3m9z7"
"ConnectionStrings": {
  "DefaultConnection": "Server=localhost;Database=VeterinariaDB;Trusted_Connection=True;"
}
```

---

### 4️⃣ Ejecutar migraciones

```bash id="p8v4s1"
dotnet ef database update
```

---

### 5️⃣ Ejecutar el servidor

```bash id="d2k6w9"
dotnet run
```

👉 API disponible en:
`https://localhost:5001` o `http://localhost:5000`

---

## 📁 Estructura del Proyecto

```id="t5y1u8"
📦 VeterinariaAPI
 ┣ 📂 Controllers
 ┣ 📂 Models
 ┣ 📂 DTOs
 ┣ 📂 Services
 ┣ 📂 Data
 ┣ 📂 Migrations
 ┗ 📄 Program.cs
```

---

## 🔌 Endpoints Principales

### 🐾 Mascotas

* `GET /api/pets` → Listar mascotas
* `POST /api/pets` → Crear mascota
* `PUT /api/pets/{id}` → Actualizar mascota
* `DELETE /api/pets/{id}` → Eliminar mascota

---

### 👤 Dueños

* `GET /api/owners`
* `POST /api/owners`
* `PUT /api/owners/{id}`
* `DELETE /api/owners/{id}`

---

### 📅 Citas

* `GET /api/appointments`
* `POST /api/appointments`

---

### 🔐 Autenticación

* `POST /api/auth/login`
* `POST /api/auth/register`

---

## 🔐 Seguridad

* Autenticación con JWT
* Validación de datos
* Protección contra inyecciones SQL
* Control de acceso por roles

---

## 🧪 Pruebas

```bash id="m1k9p3"
dotnet test
```

---

## 📬 Pruebas con Postman

Puedes probar la API usando herramientas como:

* Postman
* Thunder Client (VS Code)

---

## 🤝 Contribuciones

1. Fork del repositorio
2. Crear una rama (`git checkout -b feature/nueva-funcionalidad`)
3. Commit (`git commit -m 'Nueva funcionalidad'`)
4. Push (`git push origin feature/nueva-funcionalidad`)
5. Crear Pull Request

---

## 📜 Licencia

Este proyecto está bajo la licencia MIT.

---

## 👨‍💻 Autor

Desarrollado por **Isai Reyes**
