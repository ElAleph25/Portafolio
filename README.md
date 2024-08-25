# Portafolio

Este es mi primer portafolio para la Ciencia de Datos. El objetivo es:

- Entender la naturaleza de los problemas que presentan estos Data Sets para decidir qué algoritmo y modelo de Machine Learning aplicar para resolver dicha cuestión. 
- Limpiar y explorar los Data Sets a estudiar con base al algoritmo de Machine Learning a aplicar.
- Entrenar el algoritmo de Machine Learning.
- Generar un modelo y evaluar su eficacia.
- Dar un resumen general del problema y su modelo. 

A continuación, se ofrece el listado con los DataSets, la descripción de su problema y la resolución vía Machine Learning. 

## Modelos de Machine Learning

### Análisis semántico latente para expedientes médicos 
**Código:** [`LSA para expedientes médicos.ipynb`](https://github.com/ElAleph25/Projectos-del-Portafolio-/blob/main/LSAParaExpedientesM%C3%A9dicos/LSA%20para%20expedientes%20me%CC%81dicos.ipynb)

**Objetivo:** Realizar consultas relevantes de expedientes médicos similares.

**Descripción:**
Un problema en el sector salud, es que surja una enfermedad que provoque una epidemia, pandemia o endemia, que atente con la salud de una gran cantidad de personas en una población. Teniendo en cuenta los sintomas y características de dicha enfermedad, sería útil para los médicos y especialistas poder revisar, en sus bases de datos, los expedientes médicos de muchos pacientes y compararlos entre sí con base a las características la enfermedad. Hacer la comparación de muchos expedientes médicos similares, hace posible identificar a los pacientes con estos síntomas, para después, darles un seguimiento médico para priorizar su salud y prevenir el avance de la enfermedad. En este caso, nuestro DataSet contiene 13924 registros que son expedientes médicos. El conjunto completo de datos se encuentra en [`OHSUMED dataset`](https://www.mat.unical.it/OlexSuite/Datasets/SampleDataSets-about.htm).

El análisis semántico latente (LSA por sus siglas en inglés), es un método del "Procesamiento del Lenguaje Natural" que compara, en un corpus de textos, los documentos más similares. La metodología es, esencialmente: preprocesar y vectorizar textos, utilizar la descomposición singular de matrices
(SVD) y, finalmente, comparar los textos con la similitud del coseno. 

Es por esto que, LSA, puede ayudarnos a cumplir el propósito de comparar expedientes médicos. 

**Skills:** Preprocesamiento de texto (lemmatización y stemming), vectorizar textos (Bolsas de Palabras y TF-IDF), álgebra lineal (descomposición SVD). 

**Paquetería:** Python, Pandas, Numpy, Matplotlib, SciPy, Nltk.

**Resultados:** Al utilizar LSA que, en este caso, lo consideramos como un modelo de aprendizaje no supervisado, tenemos una forma de comparar muchos expedientes médicos. La comparación de estos textos, es con base a la similitud de frases o palabras. 
Esto puede ser de gran utilidad para los médicos que necesitan encontrar patrones, palabras y frases comúnes que cumplan un conjunto de pacientes. 

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






