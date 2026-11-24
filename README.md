# s2026q4d-acronyms-andres-jimenez
This repo contains the information fro the different acronyms assigned.

## Concepts:

### CAP – CAP Theorem: 
Es un principio de los sistemas distribuidos de almacenamiento, donde se establece que no es posible obtener las siguientes tres características simultaneamente. La primera es la consistencia (consistency), la cual indica que todos los nodos, muestran los mismos datos, si ocurre un cambio en alguno, los otros son actualizados sin inconsistencias. La siguiente es la disponibilidad (availability), la cual indica que el sistema siempre va a poder responder a las solicitudes. Por último, está la tolerancia a partición (partition tolerance), la cual indica que el sistema debe continuar funcionando ante fallos de comunicación. De esta forma, según el problema a resolver se deben priorizar dos de ellas y sacrificar una a modo de trade-off. 

**CP**: Rechaza o retrasa peticiones que no pueden ser consistentes durante una partición. 

**AP**: Continúa sirviendo durante una partición usando data local u obsoleta y reconcilia cambios luego. 

**CA**: Solo se puede conseguir cuando no hay partición de red. 

## EDA – Exploratory Data Analysis: 
El análisis exploratorio de datos implica un proceso cuya finalidad es comprender la estructura de los datos, detectar problemas de calidad, descubrir relaciones, establecer un marco con el que continuar. 

En la estructura de datos se busca observar el tamaño del dataset, nombres de columnas, tipos de datos y distribuciones de variabilidad. 

En la detección de problemas está el encontrar datos faltantes, valores duplicados, tipos de datos incorrectos y anomalías. 

En el descubrimiento de relaciones se busca analizar tendencias de datos, correlaciones entre variables y clusters de datos. 

Esto permite formular hipótesis y crear un camino a seguir con limpieza, feature engineering o técnicas de modelado. 

## DDD – Domain Driven Design: 
Es una forma de realizar el diseño de software. Establece la lógica de negocio y el dominio de conocimiento como el centro de una aplicación, es decir, busca alinear el código con la terminología de negocio, forzando un único modelo unificado entre un sistema entero. Mantiene los siguientes pilares: 

- Lenguaje ubicuo: Vocabulario preciso, compartido y sin ambigüedades. 

- Diseño estratégico: Centra el problema con sus subdominios, contextos atados y mapeo de contexto. 

- Diseño táctico: Se centra en la implementación de patrones dentro de un contexto indicando las entidades (objetos con ID cuya información persiste incluso tras cambios), objetos de valor (objetos inmutables, representan un concepto de negocio por atributos y no por ID),  

Ideal para problemas que poseen reglas de negocio amplias y complejas de gestionar con técnicas similares (por ejemplo, bancos, sistemas de salud, seguros, etc.). 

## BFF – Backend for Frontend: 
Es un patrón de arquitectura donde se busca construir un servidor de backend dedicado a cada cliente de frontend específico, en vez de dejar que todos accedan desde una única API genérica, por ejemplo segmentar entre cliente web, de móvil, smart TV, etc.truir un servidor de backend dedicado a cada cliente de frontend específico, en vez de dejar que todos accedan desde una API genérica. 

Permite distribuir la carga de archivos según el dispositivo/interfaz que consuma los servicios. Así mismo da autonomía del equipo, permitiendo que frontend pueda poseer, desplegar y escalar su propio BFF sin depender de un backend general.  

Sin embargo, genera algunos problemas como la duplicación de código y termina requiriendo más servicios a operar (cada backend individual). 
