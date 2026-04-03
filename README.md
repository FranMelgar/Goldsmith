# 🤖 Ecosistema de Automatización con IA (n8n)

Este proyecto es un sistema completo de automatización construido con **n8n**, que combina agentes de IA, bots de Telegram, RAG (Retrieval-Augmented Generation) y herramientas externas como Google Calendar, Gmail y Google Sheets.

---

## 🚀 Funcionalidades

### 📱 Bot de Telegram con IA
- Maneja mensajes de texto y voz
- Transcribe audio usando OpenAI
- Responde con IA
- Genera respuestas en audio (Text-to-Speech)
- Incluye memoria para conversaciones contextuales

---

### 🧠 Sistema de Agentes de IA
- Usa modelos de OpenAI
- Arquitectura basada en herramientas (tools)
- Soporta:
  - Búsqueda web
  - Automatización de Gmail
  - Gestión de calendario
  - Almacenamiento de contactos
  - Publicación en redes sociales

---

### 📚 RAG (Retrieval-Augmented Generation)
- Usa Pinecone como base de datos vectorial
- Responde preguntas basadas en conocimiento personalizado
- Ingesta de datos desde Google Drive
- Chunking automático + embeddings

---

### 🏪 App de Chat para Negocio (Goldsmith)
- Asistente de IA para un negocio (Gold Digger)
- Responde preguntas sobre productos/servicios
- Captura leads:
  - Nombre
  - Email
  - Teléfono
  - Intereses
- Guarda los datos en Google Sheets

---

### ☁️ MCP Server
- Funciona como servidor de herramientas
- Permite:
  - Crear y consultar eventos en Google Calendar
  - Enviar emails con Gmail
  - Leer y escribir en Google Sheets
  - Usar calculadora
  - Consultar base vectorial

---

### ⚙️ Workflows de Automatización
- Generación de contenido programado
- Pipeline Google Drive → Pinecone
- Manejo de errores con notificaciones por email

---

## 🧱 Arquitectura

```
Telegram → Agente IA → Tools → Respuesta (Texto + Audio)

Google Drive → Text Splitter → Embeddings → Pinecone

Chat App → Agente IA → RAG (Pinecone) → Respuesta

MCP Trigger → Tools (Calendar, Gmail, Sheets)
```

---

## 🛠️ Tecnologías

- n8n
- OpenAI (LLM, embeddings, TTS, STT)
- Pinecone
- Telegram API
- Google APIs (Drive, Sheets, Calendar, Gmail)

---

## 📂 Workflows incluidos

### Bot de Telegram
- Texto + voz
- Transcripción
- Respuestas con IA
- Memoria

### Sistema RAG
- Búsqueda vectorial
- Ingesta automática desde Google Drive

### MCP Server
- Integración con herramientas externas

### Workflow de errores
- Notificaciones automáticas por email

### Generador de contenido
- Automatización con IA

---

## ⚠️ Requisitos

Configurar credenciales en n8n:
- OpenAI API
- Telegram Bot API
- Google OAuth
- Pinecone API

---

## ▶️ Uso

1. Importar workflows en n8n  
2. Configurar credenciales  
3. Activar workflows  
4. Probar desde Telegram o subiendo archivos a Google Drive  

---

## 🧪 Casos de uso

- Chatbot con IA
- Generación de leads
- Asistente empresarial
- Base de conocimiento inteligente
- Automatización de tareas

---

## 🧠 Mejoras futuras

- Validación de datos
- Logging
- Rate limiting
- Mejora de prompts
- Integración frontend

---

## 👤 Autor

Fran Melgar
