# Taller de Construcción de un Agente de Investigación usando LangGraph y LangChain

Este repositorio contiene el material y el código fuente para el taller de construcción de un Agente de Investigación utilizando las librerías LangGraph y LangChain. El taller está diseñado para enseñar a los participantes cómo configurar y utilizar LangGraph para crear un agente investigativo que pueda consultar distintas fuentes de información, integrar herramientas de búsqueda y manipulación de datos, y extender la funcionalidad del agente con prompts, lógica de razonamiento y control del flujo.

## Descripción del Taller

El taller se centra en la creación de un agente investigativo que combina múltiples herramientas y fuentes de información para recopilar, analizar y presentar datos de manera estructurada y útil. El agente está compuesto por las siguientes herramientas y capacidades:

1. **ArXiv Paper Fetch**: Obtiene el resumen y los metadatos de un artículo de arXiv dado su ID.
2. **Búsqueda en la Web**: Realiza búsquedas en Google para consultas generales o para complementar la información obtenida de otras fuentes.
3. **Búsqueda RAG (Retrieval-Augmented Generation)**: Accede a una base de conocimientos local que contiene artículos de arXiv sobre IA.
4. **Búsqueda RAG con Filtro**: Realiza una búsqueda filtrada dentro de la base de conocimientos para obtener información más detallada de un artículo específico.
5. **Respuesta Final**: Presenta la información recopilada en un formato específico y fácil de entender.

## Requisitos

Para seguir este taller, necesitarás:

- Python 3.7 o superior.
- Las siguientes librerías de Python:
  - `langchain_openai`
  - `langchain_core`
  - `langgraph`
  - `langchain_community`
  - `langchain-pinecone`
  - `tavily-python`
  - `semantic-router`
  - `serpapi`
  - `google-search-results`
  - `pprintpp`
  - `python-dotenv`
  - `langchain-google-genai`
  - `tokenizers`
  - `pinecone`

Puedes instalar todas las dependencias necesarias ejecutando el siguiente comando:

```bash
pip install -r requirements.txt
```

### Variables de entorno

Asegúrate de tener un archivo `.env` en el directorio raíz del proyecto con las siguientes variables configuradas:

```env
GOOGLE_API_KEY=<TU LLAVE DE GOOGLE > #Esta llave se puede reemplazar por la que sea necesaria para el LLM de preferencia
TAVILY_API_KEY=<TU LLAVE DE TAVILY>
SERPAPI_API_KEY=<TU LLAVE DE SERPAPI>
OPENAI_API_KEY=<TU LLAVE DE OPENAI>
PINECONE_API_KEY=<TU LLAVE DE PINECONE>
```

Puedes obtener las claves de API en los siguientes enlaces:

- Google API Key: [Obtener clave de API de Google](https://ai.google.dev/gemini-api/docs/api-key)
- Tavily API Key: [Registrarse en Tavily](https://tavily.com/)
- SerpAPI Key: [Obtener clave de SerpAPI](https://serpapi.com/)
- OpenAI API Key: [Obtener clave de OpenAI](https://platform.openai.com/)
- Pinecone API Key: [Crear cuenta en Pinecone](https://www.pinecone.io/)