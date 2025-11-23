# MessagePack Full Stack Application

Aplicación full stack que demuestra el uso de diferentes formatos de serialización: JSON, MessagePack y Protocol Buffers.

## Stack Tecnológico

### Backend
- FastAPI (Python)
- MessagePack
- Protocol Buffers
- Faker (datos mock)
- Compresión: GZip, Brotli, Zstd

### Frontend
- React + TypeScript
- Vite
- Axios
- @msgpack/msgpack
- protobufjs

## Desarrollo en GitHub Codespaces

Este proyecto está configurado para funcionar en GitHub Codespaces. Al abrir el repositorio en Codespaces, se instalará automáticamente todo lo necesario.

### Ejecutar el proyecto

#### Backend
```bash
cd back
source .venv/bin/activate
uvicorn main:app --reload --host 0.0.0.0
```

El backend estará disponible en `http://localhost:8000`

#### Frontend
```bash
cd front
npm run dev -- --host
```

El frontend estará disponible en `http://localhost:5173`

## Endpoints disponibles

- `GET /data` - Retorna datos en formato según el header `Accept`:
  - `application/json` - JSON estándar
  - `application/x-msgpack` - MessagePack
  - `application/x-protobuf` - Protocol Buffers

## Características

- ✅ Generación de 500 usuarios falsos con Faker
- ✅ Soporte para múltiples formatos de serialización
- ✅ Compresión de respuestas (GZip/Brotli/Zstd)
- ✅ CORS configurado
- ✅ Interfaz React para comparar formatos
