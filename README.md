# Examen-C11-Problema-de-optimizacion-de-rutas-en-grafos-
El siguiente repositorio contiene los entregables para la prueba técnica de problema de optimización de rutas en grafos.

A continuación se presenta información del proyecto.

Se implementa el algoritmo de Dijkstra, debido a que se toma como base costos positivos, ademas de utilizar descomposición en sub-rutas, para encontrar la ruta mínima que cruza por la arista obligatoria (U,V), en general la logica que sigue el algoritmo es el siguiente S→U + Arista (U,V) + V→D.

Para la generación de datos se realizo mediante codigo python en el entorno de google colab mediante librerias **numpy**, **scipy** y **random**,si se quiere replicar en local solamente es necesario tener las librerias instaladas y tener **Python 3.8+**.

Ademas se generaron dos dataset,el primero con el objetivo de bajarlo a nivel negocio y tener un esqueleto para poder desarrollar el algoritmo teniendo un total de 6 nodos y 8 aristas, con este se realizaron pruebas y casos.

<img width="276" height="207" alt="Captura de pantalla 2026-04-29 a la(s) 5 56 51 p m" src="https://github.com/user-attachments/assets/c3d43dc9-745c-40a9-8421-578f1daf18db" />

El segundo dataset tiene el proposito para visualizar el comportamiento a nivel productivo y 
tomando como base la evolución del primer grafo añadiendo una gran cantidad de nodos y aristas y visualizando su rendimeinto computacional, para ello se genero una matriz de adyacencia dispersas, ajustando la densidad(para controlar qué tan conectada está la red) y los pesos(generando los costos) y teniendo un formato **CSR**

Supuestos

-Pesos Positivos: Se asume que todos los pesos de las aristas son positivos (necesario para el correcto funcionamiento de Dijkstra).

-Conectividad: Se asume que el grafo es lo suficientemente denso para que exista al menos una ruta válida entre los nodos seleccionados y la arista obligatoria.

-Grafo dirigido: El sistema está diseñado para tratar la arista obligatoria como un segmento direccional.






