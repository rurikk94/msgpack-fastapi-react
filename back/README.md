# Backend FastAPI con MessagePack

## Instalación

```bash
pip install -r requirements.txt
```

## Ejecutar

```bash
uvicorn main:app --reload
```

El servidor estará disponible en `http://localhost:8000`

## Endpoints

- `GET /` - Mensaje de bienvenida
- `GET /data` - Retorna datos serializados en msgpack
