# SUPERVISED-vs-UNSUPERVISED-LEARNING
Descripción general

Este conjunto de datos fue generado de forma sintética con el propósito de simular información de estudiantes universitarios y predecir si un estudiante abandonará o no su carrera durante el primer año académico.

El dataset se utiliza para aplicar modelos de Machine Learning supervisados, específicamente de clasificación binaria, como la Regresión Logística, para identificar los factores que influyen en la deserción estudiantil.

📊 Estructura del conjunto de datos

El archivo contiene 500 registros y 10 variables, divididas en tres grupos principales: demográficas, académicas, financieras, y una variable objetivo.

Tipo	Variable	Descripción	Tipo de dato	Rango / Categorías
Demográfica	edad	Edad del estudiante	Numérica	17 – 30 (algunos valores atípicos: 15, 45, 50, 60)
Demográfica	genero	Género del estudiante	Categórica	Masculino, Femenino, Otro
Demográfica	origen	Lugar de procedencia	Categórica	Local, Regional, Nacional
Académica	promedio_colegio	Promedio de notas de secundaria	Numérica	1.0 – 5.0
Académica	puntaje_admision	Puntaje en el examen de admisión	Numérica	40 – 100
Académica	nota_primer_semestre	Promedio del primer semestre	Numérica	1.0 – 5.0 (algunos atípicos: 0.2, 5.5, 6.0)
Financiera	nivel_socioeconomico	Nivel económico del estudiante	Categórica	Bajo, Medio, Alto
Financiera	beca	Indica si el estudiante posee beca o ayuda	Categórica	Sí, No
Financiera	prestamo	Indica si el estudiante tiene préstamo estudiantil	Categórica	Sí, No
Objetivo	abandono	Si el estudiante abandonó o no	Categórica	Sí, No
 Introducción de valores nulos y atípicos

Se añadieron valores nulos aleatorios en aproximadamente el 5% de los registros de cada columna, simulando la presencia de datos faltantes reales.

Se introdujeron valores atípicos (outliers) en las variables edad y nota_primer_semestre para representar posibles errores de registro o casos excepcionales.

Ejemplos: edad = 50, edad = 60, nota_primer_semestre = 0.2, nota_primer_semestre = 6.0.

Uso sugerido

Este dataset puede utilizarse para:

Entrenar modelos supervisados de clasificación (por ejemplo, Regresión Logística, Árboles de Decisión, Random Forest).

Analizar la influencia de factores académicos y financieros en la deserción.

Practicar técnicas de limpieza, manejo de valores nulos y detección de outliers.


Actividad 1 – SUPERVISED vs UNSUPERVISED LEARNING
Curso: Data Mining – Universidad de la Costa
Docente: José Escorcia-Gutiérrez
Estudiantes: Juan Pablo Cristancho Gonzalez
