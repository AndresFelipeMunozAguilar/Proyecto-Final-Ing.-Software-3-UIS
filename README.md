# **Proyecto Final de Ingeniería de Software 3**
## Análisis de performance en distintos despliegues de una aplicación de microservicios

## Introducción
En este repositorio se guardan los archivos mediante los cuales se hicieron el despliegue de la aplicación “chaphe-Bookstore-app” en distintas instancias:
  1)	Despliegue, a través del uso de Docker desktop.
  2)	Despliegue, a través del uso del componente integrado de kubernetes dentro de Docker desktop. El número de réplicas para los componentes del backend y el frontend es igual a uno.
  3)	Despliegue, a través del uso del componente integrado de kubernetes que posee Docker desktop. El número de réplicas para los componentes del backend y el frontend es igual a dos.
  4)	Despliegue, a través del uso de los componentes integrados en Docker desktop que permiten el uso de Kubernetes, para gestionar y orquestar despliegues. El número de réplicas para los componentes del backend y el frontend es igual a uno.


Se analizará el performance de la aplicación, tras realizar pruebas de carga y rendimiento con dos GUI para testing de microservicios: Postman y Jmeter

## Estructura
En esta sección se enumeran algunos archivos importantes, debido a los cuales se puede realizar el despliegue de la aplicación

1) *"Source\bookstore-app-main\backends\persistent\backend-reviews\Initialmongodb_for_docker.js."*: Este archivo permite la inserción de datos, con docker desktop y contenedores, de los datos de review de la base de datos no relacional, basada en mongo. El cambio más siginificativo es el puerto mediante el cual se conecta a la base de datos: El puerto 27017.

2) *"Planes de pruebas"*: es una carpeta que contiene los archivos de extensión *".jmx"* que, al ser ejecutados con Jmeter, permiten realizar las mismas pruebas que se realizaron a lo largo del proyecto. Incluye archivos, tanto para el despliegue en docker, como para el despliegue en kubernetes

## Referencias
- Pedraza, G. (s/f). bookstore-app: Esta aplicación de “Libreria Virtual” pretende servir como herramienta de aprendizaje de temas como microservicios, despliegue basado en contenedores (Docker) y orquestación de contenedores (Kubernetes).


## Autores
- Muñoz Aguilar Andrés Felipe - 2210087
- Osma Llanes Marisol - 2211466

