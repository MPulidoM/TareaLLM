# Tarea de LLM

En está tarea de investigación en inteligencia artificial y procesamiento de lenguaje natural (NLP), se fusionan tecnologías innovadoras como LangChain, Pinecone y OpenAI para explorar la vanguardia de la intersección entre IA y NLP. Desde la interacción dinámica con ChatGPT utilizando Python y LangChain para preguntar y recibir respuestas, hasta la creación de sistemas eficientes de recuperación y generación de respuestas (RAG) utilizando bases de datos vectoriales en memoria con Pinecone, se ha diseñado un entorno donde la eficiencia y la versatilidad convergen. Además, se han configurado RAG adicionales, aprovechando la potencia de Pinecone para administrar bases de datos vectoriales en la nube, demostrando así la amplitud de aplicaciones y la capacidad de adaptación de estas herramientas en la creación de sistemas de procesamiento de lenguaje natural avanzados. Este enfoque multidisciplinario representa un paso adelante en la investigación de tecnologías NLP y proporciona nuevas perspectivas para el desarrollo futuro en este campo.

## Empezando

El proyecto contiene:

- Se tiene la clase [Main](https://github.com/MPulidoM/TareaLLM/blob/main/main.py)  la clase LLMChain se utiliza para generar respuestas a preguntas utilizando un modelo de lenguaje y una plantilla de mensajes. La clase toma una pregunta como entrada, la formatea utilizando la plantilla de solicitud y luego pasa la solicitud formateada al modelo de lenguaje para generar una respuesta.
  
- Se tiene la clase [Memory](https://github.com/MPulidoM/TareaLLM/blob/main/memory.py) este código utiliza un modelo de lenguaje para responder una pregunta sobre la descomposición de tareas mediante la recuperación y el procesamiento de texto relevante de una página web.
  
- Se tiene la clase [Pinecote](https://github.com/MPulidoM/TareaLLM/blob/main/pinecote.py) este código utiliza un modelo de lenguaje para buscar texto relevante en un documento basándose en una consulta determinada, convirtiendo el texto y la consulta en representaciones vectoriales y recuperando los fragmentos de texto más similares de un almacén de vectores.

--> [Requerimientos](https://github.com/MPulidoM/TareaLLM/blob/main/requirements.txt) Este archivo es en el cual se tendra lo relacionado a las herramientas que es necesario instalar para el funcionamiento del proyecto de Python presentado.

## Requisitos previos

[Python](https://www.python.org/) Lenguaje de programación usado. Para ver con la versión que cuentas, Abre el CMD y pon lo siguiente:

```
python -version 
```
![image](https://github.com/MPulidoM/TareaLLM/assets/118181543/b3b88148-9894-4df9-912e-6258ae8de0ad)

Ya al tener este lenguaje puedes usar el IDE que sea de tu agrado. Opciones pueden ser [Pycharm](https://www.jetbrains.com/es-es/pycharm/) o [Visual Studio Code](https://code.visualstudio.com/)

## Arquitectura

La arquitectura de este código se basa en la cadena de lenguaje (langchain) que se compone de los siguientes componentes:

- Cargador de documentos: Se encarga de cargar los documentos relevantes para el análisis. En este ejemplo, se utiliza un cargador de texto y un cargador de base de datos web.
- Separador de texto: Divide los documentos en fragmentos más pequeños para que el modelo de lenguaje pueda procesarlos. En este ejemplo, se utiliza un separador de texto recursivo de caracteres.
- Modelo de incrustaciones de lenguaje: Convierte el texto en vectores numéricos para que puedan ser indexados y buscados eficientemente. En este ejemplo, se utiliza el modelo de incrustaciones de lenguaje OpenAI.
- Almacén de vectores: Indexa los vectores para una búsqueda eficiente. En este ejemplo, se utiliza el almacén de vectores Chroma.
- Modelo de lenguaje: Genera respuestas a las preguntas basadas en los vectores indexados. En este ejemplo, se utiliza el modelo de lenguaje OpenAI.
  
La arquitectura del código se organiza en módulos y submódulos, cada uno de los cuales se encarga de una tarea específica. El módulo principal es langchain, que contiene los módulos chains, llms, prompts, community, schema y utils. El módulo chains contiene las cadenas de lenguaje, el módulo llms contiene los modelos de lenguaje, el módulo prompts contiene los prompts, el módulo community contiene las implementaciones de la comunidad, el módulo schema contiene las clases de esquema y el módulo utils contiene las utilidades.

La arquitectura del código está diseñada para ser modular y fácil de usar, lo que permite agregar nuevos cargadores de documentos, separadores de texto, modelos de incrustaciones de lenguaje, almacenes de vectores y modelos de lenguaje según sea necesario. Además, la arquitectura del código está diseñada para ser eficiente y precisa, lo que permite  crear cadenas de lenguaje que puedan procesar y analizar grandes conjuntos de documentos. 

## Instalando

Debemos clonar el repositorio:
```
git clone https://github.com/MPulidoM/TareaLLM.git 
```
Se accede al directorio del proyecto:
```
cd TareaLLM
```
Antes de correr las clases debe tener en cuenta lo siguiente:

- La PINECONE_API_KEY de la clase [Pinecote](https://github.com/MPulidoM/TareaLLM/blob/main/pinecote.py) es obtenida de la página []()






<img width="960" alt="M1" src="https://github.com/MPulidoM/TareaLLM/assets/118181543/9d01ddce-c0e8-4f2f-bc4b-cb4dec8ba486">

<img width="960" alt="M2" src="https://github.com/MPulidoM/TareaLLM/assets/118181543/c569e80e-d04b-4b22-bdca-1e5d3e01f691">

![image](https://github.com/MPulidoM/TareaLLM/assets/118181543/19015453-1fb1-458a-bfb4-b8d294f6cf4f)




