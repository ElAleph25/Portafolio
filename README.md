# Portafolio

Este es mi primer portafolio para la Ciencia de Datos. El objetivo es:

- Entender la naturaleza de los problemas que presentan estos Data Sets para decidir qué algoritmo y modelo de Machine Learning aplicar para resolver dicha cuestión. 
- Limpiar y explorar los Data Sets a estudiar con base al algoritmo de Machine Learning a aplicar.
- Entrenar el algoritmo de Machine Learning.
- Generar un modelo y evaluar su eficacia.
- Dar un resumen general del problema y su modelo. 

A continuación, se ofrece el listado con los DataSets, la descripción de su problema y la resolución vía Machine Learning. 

## Modelos de Machine Learning

###[`Análisis semántico latente para expedientes médicos `](https://github.com/ElAleph25/Projectos-del-Portafolio-/tree/main/LSAParaExpedientesM%C3%A9dicos)



### Perceptrón para la clasificación de tejidos sanos y cancerígenos en el esófago 
**Código:** [`PerceptrónParaTejidosCancerígenos.ipynb`](https://github.com/ElAleph25/Projectos-del-Portafolio-/blob/main/Perceptr%C3%B3nParaTejidosCancer%C3%ADgenos/Perceptro%CC%81n%20Para%20Tejidos%20Canceri%CC%81genos.ipynb)

**Objetivo:** En una muestra de 5063 imágenes de tejido esofágico, clasificar los que sí tienen cáncer y los que no. 

**Descripción:** En México, el consumo de tabaco y alcohol, es muy común en adultos. El abuso de estas sustancias, comúnmente lleva a la adicción y, por consiguiente, a padecer algún tipo de enfermedad crónica en el sistema respiratorio o gástrico. Uno muy común es el cancer de esófago. 
Diagnosticar este tipo de enfermedades, regularmente se realizan a través de una biopsia mediante un videoendoscopio. Lo ideal sería que, exista una maquina que pueda, automáticamente, diagnosticar si los tejidos del esófago observados por el videoendoscopio tienen cáncer o no, ya que hacerlos visualmente con la ayuda de un especialista, resulta ser altamente costoso y tardado.

El algoritmo del Perceptrón lineal nos puede ayudar a realizar la clasificación del tejido sano y cancerígeno en automático. Este algoritmo se usará para realizar una clasificación binaria de un subconjunto de imágenes provenientes del [Data Challenge by Mauna Kea](https://challengedata.ens.fr/participants/challenges/11/).

Para este clasificador se utilizaron solamente las imágenes de tejido sano y las imágenes de tejido con displasia/cáncer.
El conjuntode datos está formado por 1,469 imágenes de tejido sano (Clase 0)  y 3,594 imágenes de displasia/cáncer (Clase 1).

Las imágenes originales fueron escaladas de 519x521 pixeles a 260x260 para reducir el tiempo y la memoria requeridos para el procesamiento. El conjunto de imágenes utilizadas están disponibles en el archivo comprimido [CarpetaImagenes.zip](https://drive.google.com/file/d/1Abi4hjl5djn8X75YCcMXL5htq7iqf7VY/view?usp=sharing), fuera de este repositorio.

**Skills:** Preprocesamiento de imágenes (vectorización de imágenes), visualización de imágenes, álgebra lineal. 

**Paquetería:** Python, Pandas, Numpy, Matplotlib, Seaborn, Sklearn, Skimage.

**Resultados:** Se obtiene un clasificador binario de tejidos cancerígenos. Este clasificador puede ser de gran utilidad para los especialistas que tratan estas enfermedades, ya que reduce el tiempo de revisión y el gran costo que tiene realizar estas pruebas. 

### Clasificación de reseñas positivas y negativas de un hotel

**Código:** [`ClasificadorReseñasRegresiónLogística.ipynb`](https://github.com/ElAleph25/Projectos-del-Portafolio-/blob/main/ClasificadorRese%C3%B1asHoteles/ClasificadorResen%CC%83asRegresio%CC%81nLogi%CC%81stica.ipynb)

**Objetivo:** En un Corpus de reseñas de hoteles de Chicago, clasificar cuáles son las reseñas positivas y cuales no. 

**Descripción:** Se utilizará regresión logistica con penalización Ridge para realizar una clasificación binaria según la autenticidad de comentarios a hoteles, utilizando un corpus de 1600 opiniones a hoteles de Chicago. 
Este corpus consiste en críticas falsas y autenticas de 20 hoteles de Chicago. Los datos fueron originalmente descritos en dos documentos de acuerdo con el sentimiento positivo o negativo de los mismos.

Este corpus contiene:

* 800 comentarios auténticos, de los cuáles 400 están clasificados como positivos y 400 como negativos
* 800 comentarios falsos, igualmente dividio en 400 comentarios positvas y 400 negativos.

**Skills:** Preprocesamiento de texto (lemmatización y stemming), vectorizar textos (Bolsas de Palabras y TF-IDF), álgebra lineal (descomposición SVD). 

**Paquetería:** Python, Pandas, Numpy, Matplotlib, SciPy, Nltk, Sklearn.

**Resultados:** Se obtiene un clasificador binario de reseñas positivas o negativas para un hotel. Este clasificador puede ser de gran utilidad para los clientes que buscan un buen lugar para pasar sus vacaciones, por ejemplo. 





