# API de Trámites — Taller 3

Gestión de Servicios en la Nube · Unidad 3 · Maestría en Gestión de Sistemas y Tecnologías de la Información (UBE)

API REST con FastAPI, autenticación JWT, pruebas con pytest e integración continua con GitHub Actions.

## Ejecutar en local

```bash
python -m venv venv
venv\Scripts\activate          # Windows  (macOS/Linux: source venv/bin/activate)
pip install -r requirements.txt
uvicorn main:app --reload
```

- Swagger UI: http://localhost:8000/docs
- Contrato OpenAPI: http://localhost:8000/openapi.json

Usuarios de prueba: `ana / ana123` y `luis / luis123`.

## Ejecutar las pruebas

```bash
pytest -v
```

## Endpoints

| Método | Ruta | Descripción | Respuesta | Protegido |
|---|---|---|---|---|
| POST | /api/v1/token | Obtiene un token de acceso | 200 OK | No |
| GET | /api/v1/tramites | Lista los trámites del usuario | 200 OK | Sí |
| GET | /api/v1/tramites/{id} | Consulta un trámite | 200 / 404 | Sí |
| POST | /api/v1/tramites | Registra un trámite | 201 Created | Sí |

## Integrantes del grupo

- (completar)
