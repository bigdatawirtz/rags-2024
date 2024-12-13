# rags-2024
Exercicio RAG

Neste repositorio podes encontrar algúns notebooks de exemplo para coñecer como funcionan os sistemas RAG.

## Instruccións

A execución dos notebooks está verficada nun Conda *environment* con Python 3.13.1. Podes reproducir este environment coas seguintes instruccións. Respecta a orde de instalación de módulos para non ter problemas de dependencias:

**Nota para equipos Ubuntu**: Se vas crear un conda environment sobre unha máquina Ubuntu asegúrate de que están instaladas as ferramentas básicas de compilación antes de instalar os módulos necesarios. Executa as seguintes liñas nunha consola de Bash:
```bash
sudo apt update
sudo apt install build-essential
```

**Creación de conda environment: rag**
```python
conda create --name rag python=3.13.1
conda install pip
pip install langchain langchain_ollama
pip install chromadb sentence-transformers langchain_huggingface langchain_chroma
pip install gradio
```

Terás que instalar a maiores algún entorno para a execución dos notebooks.

## Notebooks
- 01_ollamaLLM_prompt-basics.ipynb: Exemplo de consulta a un modelo LLM
- 02_langchain_chroma_basics-createdb.ipynb: Almacenamento de varias frases en base de datos vectorial e búsquedas de proximidade sobre os datos almacenados.
- 03_langchain_chroma_basics-readdb.ipynb: Acceso a unha base de datos vectorial con búsquedas sobre os datos almacenados.
- 04_langchain_chroma_basics-gradio.ipynb: Consulta mediante GUI (gradio) a unha base de datos vectorial.
- 05_rag_chromadb_ollama-basic.ipynb: Exemplo de sistema RAG con acceso a base de datos vectorial e elaboración de resposta mediante LLM.
