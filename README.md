# 🐈 CatTeacherBOT

[![FastAPI](https://img.shields.io/badge/Backend-FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![Discord.py](https://img.shields.io/badge/Discord-v2.0-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discordpy.readthedocs.io/)
[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)

**CatTeacherBOT** es un ecosistema multipropósito avanzado para Discord que fusiona la gestión inteligente de servidores, herramientas de ciberseguridad, entornos de aprendizaje, ejecución de código en tiempo real y análisis estadístico masivo.

El proyecto cuenta con una arquitectura híbrida: un bot altamente modular sincronizado con un **Dashboard Web** dinámico para la administración visual del sistema.

---

## 🚀 Características Clave

*   **Arquitectura Modular:** Cada módulo está separado en archivos `.py` independientes, lo que facilita el mantenimiento, la escalabilidad y la carga selectiva de extensiones (Cogs).
*   **Dashboard Integrado:** Desarrollado con **FastAPI** y plantillas **Jinja2** para visualizar estadísticas de servidores, logs en tiempo real y configuraciones analíticas.
*   **Pasarela de Criptomonedas:** Comandos integrados para gestionar donaciones y soporte del proyecto mediante wallets de criptoactivos.

---

## 📁 Estructura del Proyecto

```text
CatTeacherBOT/
│
├── main.py                 # Punto de entrada del bot y sincronización
├── app.py                  # Servidor web backend (FastAPI)
│
├── cogs/                   # Módulos y comandos del bot
│   ├── academia.py         # Sistema educativo y cursos
│   ├── admin.py            # Gestión y comandos de administración
│   ├── automod.py          # Filtros y moderación automática
│   ├── codesentinel.py     # Análisis estático y plagio de código
│   ├── ctf.py              # Competencias y retos de seguridad
│   ├── cultura.py          # Entretenimiento y menús interactivos
│   ├── ejecucion.py        # Entorno de ejecución (Shell/Linux)
│   ├── estados.py          # Control de estados del bot
│   ├── github_sentinel.py  # Integración y clonación de repositorios
│   ├── graficos.py         # Motor visual con 30 tipos de gráficos
│   ├── hacking.py          # Herramientas de auditoría y criptografía
│   ├── inteligencia.py     # Asistente y mentor de código con IA
│   ├── misiones.py         # Sistema de rachas y tareas
│   ├── notificaciones.py   # Recordatorios y alertas configurables
│   ├── permisos.py         # Control de acceso granular
│   ├── pomodoro.py         # Temporizadores de enfoque y productividad
│   ├── progreso.py         # Gamificación, XP, niveles y diplomas
│   ├── proteccion.py       # Sistema de seguridad avanzada y mitigación
│   ├── template_builder.py # Creador y clonador de plantillas
│   ├── texto.py            # Manipulación y codificación de strings
│   ├── utilidades.py       # Herramientas del día a día y matemáticas
│   └── vuln.py             # Base de datos de exploits y vulnerabilidades
│
├── templates/              # Vistas HTML del Dashboard (Jinja2)
└── static/                 # Archivos CSS, JS e imágenes del panel
