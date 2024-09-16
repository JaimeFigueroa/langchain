# Agentes y RAG en LangChain  

Notas personales basadas en la [documentación oficial](https://python.langchain.com/v0.2/docs/introduction/) de LangChain.

El código lo puedes encontrar en la carpeta `notebooks` de este repo.

<br/>

## ¿Qué eson los agentes?  
En terminos sencillos, son modelos de IA que tienen la capacidad de interactuar con otros servicios. Son el resultado de aplicar metodolgías de desarrollo de sistemas a los modelos de lenguaje natural (LLMs). 

<br/>

## ¿Porqué LangChain?  
Al día de hoy (2024), los modelos de lenguaje natural tienen limitaciones importantes que limitan su aplicación directa en procesos de negocio. 

LangChain es un framework que busca atacar estas limitaciones al brindar a los modelos con herramientas para interactuar con otros servicios.

<br/>

## ¿Que significa RAG?
La Generación Aumentada por Recuperación (RAG por sus siglas en inglés) es una tecnica que busca atacar la limitación en cuestion de tamaño de la ventana de contexto y el de la fiabilidad y vigencia de los datos entregados por el modelo.

Al aplicar un proceso RAG se busca mejorar las respuestas obtenidas al proporcionar al modelo información relevante (almacenada en fuentes externas) antes de que este genere su respuesta.

<br/>

## ¿Qué es Chroma?
Chroma es una base de datos que nos permite buscar información usando un espacio vectorial de N dimensiones como indice. Al utilizar encodings generados por un modelo de lenguaje como índices en Chroma, podemos almacenar fragmentos de un documento en una base de datos para después utilizar el encoding de la pregunta para localizar los fragmentos con el contexto más relevantes antes de generar la respuesta.

