# HR Agent — Telegram Bot

Agente conversacional de HR que opera por Telegram en lenguaje natural. 
Los empleados escriben lo que necesitan y el agente lo ejecuta automáticamente.

## Qué hace
- Registra novedades de nómina (aumentos, horas extra, bonos, reembolsos)
- Genera certificados laborales en PDF y los envía por Telegram automáticamente
- Gestiona solicitudes de permisos, logística y documentos
- Responde preguntas frecuentes sobre procesos internos
- Mantiene memoria conversacional para interacciones naturales

## Stack
- **Telegram** — canal de interacción
- **n8n** — orquestación del flujo
- **OpenAI GPT-4o** — interpretación de intenciones y generación de respuestas
- **Supabase** — base de datos (empleados, novedades, solicitudes, historial)
- **Google Sheets** — vista operativa para el equipo de HR
- **PDFShift** — generación de PDFs

## Arquitectura
El agente recibe mensajes en lenguaje natural, consulta el historial 
de conversación para mantener contexto, interpreta la intención con GPT-4o, 
y enruta la solicitud según su tipo para ejecutar la acción correspondiente.
