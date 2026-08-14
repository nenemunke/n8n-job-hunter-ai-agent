# 🤖 Autonomous AI Job Hunter & Tech Radar (n8n + Gemini + Tavily)

Pipeline de automatización de inteligencia laboral y vigilancia tecnológica diseñado con **n8n**, **Google Gemini** y **Tavily Web Search**, con entrega periódica mediante bot de **Telegram**.

## 📌 Arquitectura del Sistema
- **Orquestador:** n8n (Self-hosted via Docker).
- **LLM Engine:** Google Gemini 3.5 Flash Lite (Reasoning & Data Extraction).
- **Search Tooling:** Tavily Search API.
- **Alert Channel:** Telegram Bot API (Parse Mode: HTML).

## ⚙️ Reglas de Negocio Implementadas
- **Filtro de cargos:** Desarrollo de software, AI Engineering, Data Science / Analytics, Soporte de software & QA.
- **Filtro de funciones:** Exclusividad para roles con contacto directo con código (requerimiento académico).
- **Priorización geográfica:** Región Metropolitana (Remoto), Ñuble (Presencial), Biobío (Híbrido/Presencial).
- **Ventana temporal:** Ofertas de los últimos 4 días para evitar vacantes caducadas.

## 🚀 Cómo importarlo
1. Clonar este repositorio.
2. En n8n: Menú superior -> `Import from File` -> Seleccionar `workflows/job_market_ai_agent.json`.
3. Configurar las credenciales de Gemini, Tavily y Telegram.
4. Activar el workflow.
