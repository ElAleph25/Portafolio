# Portafolio

Este es mi primer portafolio para la Ciencia de Datos. El objetivo es:

- Entender la naturaleza de los problemas que presentan estos Data Sets para decidir qué algoritmo y modelo de Machine Learning aplicar para resolver dicha cuestión. 
- Limpiar y explorar los Data Sets a estudiar con base al algoritmo de Machine Learning a aplicar.
- Entrenar el algoritmo de Machine Learning.
- Generar un modelo y evaluar su eficacia.
- Dar un resumen ejecutivo general del problema y su modelo. 

A continuación, se ofrece el listado con los DataSets, la descripción de su problema y la resolución vía Machine Learning. 

## Modelos de Machine Learning

### Análisis semántico latente para expedientes médicos 
**Código:** [`LSA para expedientes médicos.ipynb`](https://github.com/tiannaparris/PortfolioProjects/blob/main/Analyzing%20the%20Factors%20Contributing%20to%20the%20Success%20of%20a%20Movie.ipynb)

**Objetivo:** Realizar consultas relevantes de expedientes médicos similares.

**Descripción:**
Un problema común que podría tener el sector salud, es que exista una epidemia (como la del COVID) que atente con la salud de una gran cantidad de personas. Teniendo en cuenta los sintomas (o características) de dicha enfermedad, sería útil para los médicos poder revisar, rápidamente, los expedientes médicos de muchos pacientes y compararlos entre sí con base a las características de la epidemia. Una vez identificados estos expedientes similares, es posible darles un seguimiento médico a estos pacientes para prevenir el avance de la enfermedad. En este caso, nuestro DataSet contiene 13924 registros que son expedientes médicos. 

El análisis semántico latente (LSA por sus siglas en inglés), es un método del "Procesamiento del Lenguaje Natural" que compara, en un corpus de textos, los documentos más similares. La metodología es, esencialmente: preprocesar y vectorizar el texto, utilizar la descomposición singular de matrices
(SVD) y, finalmente, comparar los textos con la similitud del coseno. 

**Skills:** Preprocesamiento de texto (lemmatizar y stemizar), vectorizar textos (TF-IDF), álgebra lineal (descomposición SVD). 

**Paquetería:** Python, Pandas, Numpy, Matplotlib, SciPy.

**Resultados:** Al utilizar LSA, tenemos una forma de comparar muchos expedientes médicos. La comparación de estos textos, es con base a la similitud de frases o palabras. 
Esto puede ser de gran utilidad para los médicos que necesitan encontrar patrones, palabras y frases comúnes que cumplan un conjunto de pacientes. 


