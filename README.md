# 📅 Automatizador Diario de Tareas con n8n

Este proyecto automatiza el proceso de enviar un correo diario con las 3 tareas más prioritarias desde una hoja de cálculo de Google Sheets, utilizando **n8n Community Edition** autoalojado.

## 🚀 ¿Qué hace?

- Lee todas las tareas de una hoja de Google Sheets
- Filtra las que están marcadas como "pendiente"
- Ordena por prioridad (Alta > Media > Baja)
- Elige las 3 más importantes
- Envía un correo con la lista formateada

## 📋 Requisitos

- Cuenta de Google con acceso a:
  - Google Sheets (con hoja `Tareas`)
  - Gmail
- Hoja con columnas:
  - `Tarea`
  - `Prioridad` (`Alta`, `Media`, `Baja`)
  - `Estado` (`pendiente`, `completado`, etc.)
- n8n (Community Edition) instalado localmente con acceso a internet
- Credenciales OAuth2 configuradas para Gmail y Google Sheets

## 🛠️ Instalación

1. Clona este repositorio:
   ```bash
   git clone https://github.com/tuusuario/n8n-tareas-diarias.git
   cd n8n-tareas-diarias
2. Abre tu n8n local en el navegador

3. Crea tus credenciales de Google (OAuth2)

4. Importa el archivo JSON desde:
    workflow/agendador-diario-tareas.json
  
5. Conecta tus credenciales manualmente

6. Ajusta el horario desde el nodo Schedule Trigger

7. Haz clic en Activate para que se ejecute automáticamente
