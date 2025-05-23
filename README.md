# ElectoAI – Asistente Electoral Inteligente

**ElectoAI** es una aplicación basada en inteligencia artificial diseñada para responder dudas legales y operativas durante el proceso electoral en la Ciudad Autónoma de Buenos Aires (CABA) 2025.

El sistema está construido con técnicas de **Retrieval-Augmented Generation (RAG)** y utiliza modelos de lenguaje locales o en la nube para interpretar consultas y brindar respuestas claras, actualizadas y confiables.

---

## 🧠 ¿Qué puede responder?

ElectoAI puede asistir a:

- Jueces y autoridades de mesa  
- Fiscales partidarios  
- Ciudadanos que participan del proceso electoral

**Ejemplos de consultas**:
- ¿Cuándo se vota?
- ¿Qué documentos son válidos para votar?
- ¿Qué hacer si faltan boletas?
- ¿Quién encabeza la lista de tal partido?
- ¿Puede ingresar alguien con una remera partidaria?

---

## 🛠️ Tecnologías utilizadas

- **LangChain** para la construcción del pipeline RAG  
- **Chroma** como vector store local  
- **HuggingFace embeddings** para codificar texto  
- **Gradio** como interfaz (opcional)  
- **Modelos LLM locales (como Mistral en Ollama)** o GPT vía OpenAI  

---

## 🚀 Cómo ejecutar el proyecto

1. Cloná este repositorio:
   ```bash
   git clone https://github.com/tuusuario/electoai.git
   cd electoai
   ```

2. Instalá las dependencias:
   ```bash
   pip install -r requirements.txt
   ```

3. Abrí la notebook principal:
   ```
   Elecciones.ipynb
   ```

> Asegurate de tener un archivo `.env` configurado si usás OpenAI.

---

## 📁 Estructura del proyecto

```
.
├── knowledge-base/       # Documentos cargados (PDF, MD, TXT, etc.)
├── vector_db/            # Base de datos vectorial persistente (Chroma)
├── .env                  # Claves de API y configuración local (no versionado)
├── requirements.txt      # Dependencias del proyecto
├── runtime.txt           # Versión de Python requerida
└── Elecciones.ipynb      # Notebook principal
```

---

## 📄 Licencia

Este proyecto es de uso educativo y experimental. Consultá las condiciones de uso de los modelos LLM y embeddings que elijas integrar.
