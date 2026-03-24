# Hito 3: Automatización Inteligente con n8n + Ollama + PostgreSQL + Qdrant

Desarrollo de Agentes IA para Web - 2º DAW
IES Iliberis - Profesora: Ana María Fuentes Conde

## Descripción

Este proyecto contiene la infraestructura y configuración para desarrollar dos sistemas:
1. **Sistema RAG**: Procesa documentos, los vectoriza y permite hacer preguntas.
2. **Chatbot Multiherramienta**: Asistente conversacional que consulta APIs (Meteo, Wikipedia, Países, Chistes).

## Estructura

- `docker/`: Configuración para levantar PostgreSQL mediante Docker Compose. (Se asume que n8n, qdrant y ollama ya están corriendo localmente).
- `n8n/workflows/`: Archivos `.json` listos para ser importados en n8n.
- `postgres/`: Script SQL de inicialización `init.sql`.
- `tests/`: Peticiones en formato HTTP (`pruebas.http`) para probar las APIs.
- `docs/`: Archivos para documentar la entrega (`DEMO.md` y carpeta `capturas`).

## Despliegue Rápido
1. Copiar `.env.example` a `.env` en la carpeta `docker` y ajustar valores si se requiere.
2. Ejecutar `docker-compose up -d` dentro de la carpeta `docker` para levantar PostgreSQL.
3. Importar los flujos `.json` de `n8n/workflows` en la interfaz de n8n.
