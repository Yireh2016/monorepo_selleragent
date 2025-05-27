# Monorepo: Vite + SolidJS Frontend & Django Backend

## Structure
- `frontend/`: Vite SPA with SolidJS, TypeScript, Vitest, and Tailwind CSS
- `backend/`: Django backend

## Getting Started

### Frontend (with Tailwind CSS)
We use [Tailwind CSS](https://tailwindcss.com/) for utility-first styling in the frontend. You can use Tailwind classes in your SolidJS components.

#### Local Development
```sh
cd frontend
npm install
npm run dev
```

#### Frontend Tests
```sh
cd frontend
npm run test
```

### Backend
```sh
cd backend
python manage.py migrate
python manage.py runserver
```

## Running with Docker Compose
You can run both frontend and backend (with hot reload) using Docker Compose:

```sh
docker-compose up --build
```
- Frontend: http://localhost:5173 (hot reload enabled)
- Backend: http://localhost:8000 (auto-reload enabled)

> Changes to your code will be reflected automatically in the running containers.

## API Documentation (Swagger/OpenAPI)
After starting the backend, you can view the interactive API docs at:

- Swagger UI: http://localhost:8000/api/schema/swagger-ui/
- ReDoc: http://localhost:8000/api/schema/redoc/
- Raw OpenAPI schema (JSON): http://localhost:8000/api/schema/

## Communication
Use REST APIs or similar to connect frontend and backend.
