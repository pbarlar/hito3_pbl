# Demostración del Hito 3

Este documento servirá para almacenar las evidencias del funcionamiento del sistema.

## Proyecto A: Sistema RAG Educativo

### 1. Ingesta de Documentos
- [ ] Captura de n8n mostrando la ejecución exitosa del workflow de ingesta.
- [ ] Captura de la base de datos PostgreSQL (`documentos`) con el registro insertado.
- [ ] Captura opcional de Qdrant mostrando los vectores creados.

*Insertar imagen aquí: `![Ingesta](../capturas/n8n-ingesta.png)`*

### 2. Consultas RAG
- [ ] Captura de una petición exitosa preguntando sobre el documento y la respuesta.
- [ ] Captura de la base de datos PostgreSQL (`consultas_rag`).

*Insertar imagen aquí: `![Consulta RAG](../capturas/n8n-rag-consulta.png)`*

---

## Proyecto B: Chatbot Multiherramienta

### 1. Enrutamiento Inteligente (Switch)
- [ ] Captura del flujo en n8n donde Ollama decide qué herramienta instanciar basado en una pregunta (Ej: "Dime el clima en Madrid").
- [ ] Captura de la consulta a la API de Wikipedia ("¿Quién fue Cervantes?").
- [ ] Captura de la respuesta enviada al usuario.
- [ ] Captura de PostgreSQL demostrando que la conversación se guardó en `historial_chatbot`.

*Insertar imagen aquí: `![Chatbot](../capturas/n8n-chatbot.png)`*
