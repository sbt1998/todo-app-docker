# 📝 Todo App — Flask + PostgreSQL

Aplicación web CRUD de lista de tareas con Python/Flask y base de datos PostgreSQL.

## 🚀 Arranque rápido (Docker)

```bash
./start.sh
```

O directamente:

```bash
docker compose up --build
```

Abre el navegador en: `http://localhost:5000`

## 🛠️ Tecnologías

- **Backend:** Python 3.11 + Flask
- **Base de datos:** PostgreSQL 15
- **Contenedores:** Docker + Docker Compose

## 📦 Estructura

```
todo-app/
├── app/
│   ├── app.py           # Aplicación Flask
│   ├── requirements.txt # Dependencias Python
│   └── Dockerfile       # Imagen del backend
├── docker-compose.yml   # Orquestación Docker
├── start.sh             # Script de arranque
└── .devcontainer/       # Config GitHub Codespaces
```

## 🔌 API REST

| Método | Ruta | Descripción |
|--------|------|-------------|
| GET | `/api/tasks` | Listar tareas |
| POST | `/api/tasks` | Crear tarea |
| PUT | `/api/tasks/:id/toggle` | Marcar como hecha/pendiente |
| DELETE | `/api/tasks/:id` | Eliminar tarea |
