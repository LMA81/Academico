# Proyecto Desempeño Académico
El presente proyecto buscó dar cuenta de una propuesta de investigación para el curso Analítica de Datos contenido en el programa; Diploma en Ciencia de Datos Avanzados, Universidad de Concepción,2019).

El objetivo del estudio es identificar los principales predictores (variables) de éxito y riesgo académico que mejor se ajustan y explican la predicción de la deserción académica dada una preclasificación del estudiantado. 

El DataSet es de carácter histórico (2000-2017) con data de caracterización de ingreso del estudiantado y de la progresión académica durante el respectivo proceso formativo. La data se encuentra contenida en 5 archivos:
1.	ADMISIÓN; contiene información referente a las condiciones de ingreso del estudiante a la carrera, tales como; puntajes PSU (ponderado y desglosado por matemática, lenguaje y ciencia), ponderación NEM, el tipo de colegio de egreso (particular, subvencionado, municipalizado), dato demográfico, entre otros.
2.	ALUMNOS INSCRITOS POR ASIGNATURAS (Alu-Insc-Asi); dada la dimensión del dataset está dividida en tres pac c/u contiene información semestral de las asignaturas cursadas con las evaluaciones obtenidas por el estudiantado.
3.	ASIGNATURAS COMPLEMENTARIAS; oferta de asignaturas complementaria ofrecida con información relativa a; nombre asignatura, unidad académica que la imparte, duración, número de créditos, horas semanales (teóricas, laboratorio y practicas), entre otros.
4.	RENDIMIENTO; contiene información cruzada entre la data contenida en el DataSet Admisión con el DataSet Situación.
5.	SITUACIÓN; estado académico actual del estudiantado (alumno regular, baja académica, baja por no inscripción, suspensión de estudio autorizada, autorizado para titularse, titulado, etc).

Restricción del estudio: existe una preclasificación del estudiantado; “Bueno Estudiante” (Se Titula), “Muy Buen Estudiante” (Se Titula a lo más en T+1 años, donde T= duración carrera declarada) y “Excelente Estudiante” (Se Titula en tiempo T).

El propósito se centrará en determinar una clasificación, de forma tal que logre identificar cuál combinación de variables explica, en mayor medida, la clasificación predefinida. Para tales efectos, se decide trabajar con los archivos admisión, rendimiento y situación, dado que estos concentran la principal información para poder determinar tanto el perfil de egreso e ingreso del estudiante, como las variables que se encuentran correlacionadas entre ambos perfiles.

En resumen, se clasifica estudiantado de acuerdo a la restricción predeterminada, a cada preclasificación se asignan todas las variables para luego identificar aquellas que tengan mayor peso en dicha clasificación. Para tales efectos, se usa aprendizaje supervisado algoritmos de árbol de decisión en particular se usa Decision Tree y Random Forest. Siendo este último el mejor algoritmo (accuracy 76% v/s 74%) para obtener la importancia de cada variable en explicar el modelo.

Este trabajo fue realizado junto a Edgardo Cabrera, utilizando el lenguaje de programación Python.

NOTA: EL DATASET Y CODIGO NO ESTÁ DISPONIBLE DEBIDO A LA SENSIBILIDAD DE SU CONTENIDO.
