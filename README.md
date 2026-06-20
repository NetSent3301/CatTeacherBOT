# 🐈 CatTeacherBOT — Enterprise Discord Ecosystem

[![FastAPI](https://img.shields.io/badge/Backend-FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![Discord.py](https://img.shields.io/badge/Discord-v2.0+-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discordpy.readthedocs.io/)
[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

**CatTeacherBOT** es un ecosistema multipropósito avanzado diseñado para Discord. Fusiona entornos de aprendizaje interactivo, herramientas de auditoría de seguridad y pentesting, simulación de CTFs, un motor de renderizado estadístico de 30 gráficos, moderación defensiva de alta granularidad y un sistema completo de gamificación.

El núcleo está desarrollado bajo una **arquitectura híbrida síncrona**, donde el bot se conecta directamente a una API/Dashboard Web responsivo potenciado por **FastAPI** y **Jinja2**.

---

## 🚀 Arquitectura del Sistema

*   **Modularidad Avanzada:** Arquitectura modular basada en extensiones independientes, permitiendo el hot-reload (recarga en caliente) de herramientas específicas sin interrumpir el servicio general.
*   **Web Dashboard Sincronizado:** Rutas asíncronas para visualización de analíticas de servidores, logs en tiempo real y configuraciones globales mediante peticiones a la API local.
*   **Crypto Gateways:** Abstracción de comandos listos para gestionar flujos y logs de donaciones mediante Web3/crypto wallets.

---

## 📖 Desglose Técnico de Funcionalidades y Comandos

*El prefijo por defecto del sistema es `.` (configurable a través de comandos globales).*

### 🎓 1. Academia e Inteligencia Artificial
Módulos enfocados a la capacitación técnica y resolución de problemas algorítmicos.
*   **Comandos Académicos:** `.ejercicio`, `.solucion`, `.curso`, `.lenguajes`, `.sintaxis`, `.algoritmo`, `.nota`, `.tutorial`, `.examen` (o `.test`), `.clase`, `.libro`, `.dcl`, `.proyecto`.
*   **Comandos de Inteligencia Artificial:** `.ia`, `.explica`, `.duda`, `.ayudacodigo`, `.logica`, `.estudiar`, `.repasar`, `.aprender`, `.mentor`, `.suggest` (o `.sugerir`), `.aimodo` (o `.aimode`), `.intel`.

### 🛡️ 2. Auditoría, Redes y Ciberseguridad
Suite ofensiva-defensiva emulada e integrada para fines pedagógicos y técnicos.
*   **Grupo `.hack`:** `.hack nmap`, `.hack dns`, `.hack whois`, `.hack nikto`, `.hack dirb`, `.hack headers`, `.hack hash`, `.hack encrypt`, `.hack decrypt`.
*   **Grupo `.vuln`:** `.vuln search` (búsqueda de CVEs), `.vuln info`, `.vuln exploit` (o `.exploits`), `.vuln latest` (vulnerabilidades de última hora).
*   **Grupo `.ctf`:** `.ctf list`, `.ctf start`, `.ctf submit`, `.ctf hint`, `.ctf skip`.

### 💻 3. Entorno de Ejecución y Análisis de Código
Entorno de control, testing y debugging de código directo en canales de Discord.
*   **Ejecución Nativa:** `.run` (o `.correr` / `.ejecutar`), `.sh`, `.shell`, `.linux`.
*   **Grupo `.code` (Análisis Dinámico):** `.code analyze`, `.code complexity` (Métrica de Complejidad Ciclomática), `.code submit`, `.code compare`, `.code plagiarism` (o `.plagio`), `.code explain`, `.code run`.
*   **Grupo `.github` (o `.gh`):** `.gh repo`, `.gh langs`, `.gh readme`, `.gh raw`, `.gh clone`, `.gh pr`.

### 📊 4. Motor Estadístico y Gráficos
Soporta **30 subcomandos** dedicados a la visualización de datos usando librerías de análisis de datos estructurados, renderizando las imágenes vectorizadas al chat mediante el grupo **`.grafico`** o **`.graph`**:
*   *Estadísticos Básicos:* `bar`, `line`/`linea`, `pie`/`torta`/`pastel`, `scatter`/`dispersion`/`puntos`, `histogram`/`histograma`, `boxplot`/`caja`/`bigotes`, `area`, `stacked`/`apilado`, `donut`/`dona`.
*   *Avanzados / Ingeniería:* `funcion`/`func`/`function`/`formula`/`ecuacion`/`plot`, `radar`/`arana`, `heatmap`/`calor`, `treemap`/`arbol`, `sankey`, `kpi`/`indicador`/`gauge`, `mapa`/`map`, `violin`/`violinplot`, `bubble`/`burbujas`, `waterfall`/`cascada`, `contour`/`contorno`, `tabla`/`table`, `json`/`json_viewer`.
*   *Estructura y Procesos:* `mindmap`/`mapa_mental`, `flowchart`/`diagrama_flujo`, `tree`/`arbol_h`, `progreso`, `ranking`, `lenguaje`/`lenguajes`/`lang`, `horas`/`hora`/`actividad`.

### ⚙️ 5. Administración del Sistema y Escalado de Privilegios
Herramientas directas de ejecución en la máquina host y control de la infraestructura interna de Discord.
*   **Comandos Directos Core:** `setownerrole`/`ownerrole`, `setadminrole`/`adminrole`, `say`, `dm`/`privado`, `purge`/`clean`, `reload`/`recargar` (Hot-reload de módulos), `sync` (Sincronización de comandos de barra de Discord), `setprefix`/`prefix`, `eval`/`py`/`exec` (Evaluador de expresiones en tiempo real), `sql`/`db` (Interrogación directa de base de datos), `servidores`/`guilds`, `botinfo`/`bot`, `audit`, `server`/`guild`, `nuke`, `ban`, `kick`, `mute`/`timeout`, `unmute`/`untimeout`, `warn`, `close`, `sudo`.
*   **Grupo `.role` (o `.rol`):** `.rol create`/`crear`, `.rol delete`/`eliminar`, `.rol add`/`asignar`, `.rol remove`/`quitar`, `.rol list`/`lista`, `.rol color`.
*   **Grupo `.channel` (o `.canal`):** `.canal create`/`crear`, `.canal delete`/`eliminar`, `.canal rename`/`renombrar`, `.canal topic`/`tema`, `.canal slowmode`.
*   **Grupo `.autorole` (o `.autorol`):** `.autorol set`, `.autorol remove`, `.autorol check`, `.autorol list`, `.autorol add`, `.autorol delete`, `.autorol sync`, `.autorol scan`, `.autorol classify`.
*   **Grupo `.permiso`:** `.permiso add`, `.permiso remove`/`del`/`delete`/`rm`, `.permiso list`/`ls`/`show`, `.permiso default`, `.permiso all`.

### 🛡️ 6. Suite de Mitigación, Protección y AutoMod
Sistemas de seguridad reactiva y proactiva frente a ataques automatizados, raids e infracciones de políticas del servidor.
*   **Grupo `.automod`:** `.automod help`, `.automod config`, `.automod verifyrole`/`vr`, `.automod memberrole`/`mr`, `.automod mutedrole`/`mutrole`, `.automod verifychannel`/`vc`, `.automod alertchannel`/`ac`, `.automod logchannel`/`lc`, `.automod filter`, `.automod whitelist`, `.automod unwhitelist`, `.automod check`/`info`/`user`, `.automod verify`/`v`.
*   **Grupo `.mod` (35 Subcomandos Defensivos):** `.mod help`, `.mod config`, `.mod report`/`reporte`, `.mod investigate`/`investigar`/`check`, `.mod history`/`historial`, `.mod immunity`/`inmunidad`, `.mod logs`, `.mod lockdown`, `.mod unlock`/`unlockdown`, `.mod slowmode`, `.mod timeout`, `.mod warn`, `.mod strike`, `.mod unrestrict`/`liberar`, `.mod jail`/`aislar`, `.mod release`/`liberarjail`, `.mod whitelist`, `.mod unwhitelist`, `.mod blacklist`, `.mod unblacklist`, `.mod filter`, `.mod threshold`, `.mod action`, `.mod punishments`/`castigos`/`penalties`, `.mod scan`, `.mod purge`, `.mod alert`, `.mod logchannel`/`log`, `.mod nuke`, `.mod cleanup`, `.mod masskick`, `.mod voicekick_all`/`vkickall`, `.mod hardban`, `.mod net`/`geoip`/`dns`, `.mod timeline`/`eventos`, `.mod autoharmony`/`auditar`/`harmony`, `.mod quarantine`/`cuarentena`, `.mod unquarantine`/`liberarqr`.

### 📈 7. Gamificación, Retención y Enfoque
Diseñado para incentivar la participación continua de los usuarios y el control del tiempo enfocado.
*   **Módulo de Crecimiento y Progreso (20 Comandos):** `.hecho`, `.estudiante`, `.perfil`, `.xp`, `.nivel`, `.rango`, `.logro`/`.logros`, `.medalla`, `.ranking`/`.top`, `.meta`, `.estadisticas`, `.historial`, `.mision`, `.diario`, `.semanal`, `.mensual`, `.recompensa`/`.rewards`, `.diploma`, `.puntos`, `.lenguaje`/`.lang`.
*   **Módulo de Rachas y Misiones:** `.misiones`/`.semanales`, `.racha`/`.streak`, `.checkin`/`.check`.
*   **Grupo `.pomodoro` (o `.pomo`):** `.pomo iniciar`/`start`/`empezar`, `.pomo parar`/`stop`/`cancelar`, `.pomo estado`.

### 🧰 8. Utilidades, Manipulación de Texto y Helpers
Herramientas secundarias utilitarias de uso diario y entretenimiento.
*   **Módulo de Texto (19 Comandos):** `.mayus`, `.minus`, `.reves`, `.longitud`, `.palabras`, `.vocales`, `.consonantes`, `.espacios`, `.palindromo`, `.anagrama`, `.morse`, `.binario`, `.hex`, `.base64`, `.ascii`, `.limpiar`, `.reemplazar`, `.cifrar`, `.descifrar`.
*   **Módulo de Utilidades (20 Comandos):** `.ping`, `.hora`, `.fecha`, `.dado`, `.moneda`, `.azar`, `.sumar`, `.restar`, `.multiplicar`, `.dividir`, `.calculadora`, `.alarma`, `.temporizador`, `.cronometro`, `.clima`, `.dolar`, `.cripto`, `.passgen`, `.qr`, `.eco`.
*   **Grupo `.recordatorio`:** `.recordatorio on`/`si`/`activar`, `.recordatorio off`/`no`/`desactivar`, `.recordatorio cada`/`intervalo`.
*   **Grupo `.template` (o `.tpl` / `.templates`):** `.template create`, `.template clone`, `.template browse`/`explorar`, `.template list`, `.template delete`, `.template cancel`.
*   **Estados y Entretenimiento:** `.estado`/`.modo`/`.state`, `.comandos` (Menú interactivo global), `.chiste`/`.joke`/`.risa`.

---

## 🛠️ Despliegue e Instalación

### Requisitos Mínimos
*   Python 3.10 o superior.
*   Token de Bot de Discord (obtenido en Discord Developer Portal).
*   Variables de entorno configuradas (`.env`).

### Pasos de Configuración
1. **Clonar el repositorio:**
```bash
   git clone [https://github.com/tu-usuario/CatTeacherBOT.git](https://github.com/tu-usuario/CatTeacherBOT.git)
   cd CatTeacherBOT
