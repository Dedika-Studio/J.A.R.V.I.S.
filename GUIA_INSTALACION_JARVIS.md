# 🚀 Guía de Instalación: J.A.R.V.I.S. (Skyvern + Ollama)

Esta guía te ayudará a instalar y configurar tu propio asistente **J.A.R.V.I.S.** en tu PC de forma **100% gratuita** utilizando **Ollama** como motor de Inteligencia Artificial.

---

## 📋 Requisitos Previos

Antes de empezar, asegúrate de tener instalado:
1. **Python 3.11** (Recomendado)
2. **Node.js** (Versión 18 o superior)
3. **Git**

---

## 🛠️ Paso 1: Instalar Ollama (El Cerebro)

Ollama es el motor que ejecutará la IA localmente en tu PC.

1. Descarga Ollama desde [ollama.com](https://ollama.com).
2. Instálalo y ejecútalo.
3. Abre una terminal (CMD o PowerShell) y descarga el modelo de IA:
   ```bash
   ollama pull neural-chat
   ```

---

## 📂 Paso 2: Clonar el Repositorio

1. Abre una terminal y clona tu repositorio:
   ```bash
   git clone https://github.com/Dedika-Studio/J.A.R.V.I.S.
   cd J.A.R.V.I.S.
   ```

---

## ⚙️ Paso 3: Configurar el Entorno

1. Crea un entorno virtual de Python:
   ```bash
   python -m venv venv
   source venv/bin/activate  # En Windows usa: venv\Scripts\activate
   ```
2. Instala las dependencias:
   ```bash
   pip install skyvern
   ```
3. Crea un archivo llamado `.env` en la carpeta raíz y pega lo siguiente:
   ```env
   # --- OLLAMA (LOCAL, 100% GRATUITO) ---
   ENABLE_OLLAMA=true
   OLLAMA_MODEL_NAME=neural-chat
   OLLAMA_API_BASE=http://localhost:11434

   # --- DESACTIVAR OTROS PROVEEDORES ---
   ENABLE_OPENAI=false
   ENABLE_ANTHROPIC=false
   ENABLE_OPENAI_COMPATIBLE=false
   ENABLE_GROQ=false
   ```

---

## 🚀 Paso 4: Ejecutar J.A.R.V.I.S.

1. Inicia el servidor de Skyvern:
   ```bash
   skyvern quickstart
   ```
2. Abre tu navegador en `http://localhost:8080`.

---

## 💡 Consejos de Uso

- **Memoria RAM**: Asegúrate de tener al menos 8GB de RAM para que el modelo de IA funcione con fluidez.
- **Automatización**: Puedes pedirle a J.A.R.V.I.S. que realice tareas como:
  - "Busca las últimas noticias de tecnología en Google y haz un resumen."
  - "Entra en Amazon, busca 'teclado mecánico' y extrae los precios del primer resultado."

---

¡Listo! Ya tienes tu propio **J.A.R.V.I.S.** funcionando localmente y gratis. 🤖✨
