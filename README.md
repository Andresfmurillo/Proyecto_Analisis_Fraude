# Proyecto_Analisis_Fraude


Objetivos del proyecto

1.	Determinar patrones para la detección y prevención de fraude.
2.	Crear un sistema de indicadores, para la detección de actividades sospechosas
3.	Implementar los algoritmos de detección de patrones, para el aprendizaje del sistema



### Proceso de Calidad de Datos

Exploración de los Datos	
Pruebas para la Detección del Fraude
1.	Test IGUAL-IGUAL-IGUAL
2.	Test IGUAL-IGUAL-DIFERENTE 
3.	Rangos Intercuartílicos 
4.	Regresión Logística
5.	Regresión Logística y uso de Ridge y Lasso
6.	K-Neighbors
7.	Árbol de Decisión
8.	Random Forest
9.	Métricas comparativas de los Modelos


### Conclusiones

▪	El proceso de exploración, depuración y de examinación en general de los datos del proyecto, es el primer paso y es sumamente necesario con el fin de garantizar o lograr alta calidad de los datos que van a ser usados en el proyecto de analitica. 

▪	Los test IGUAL-IGUAL-IGUAL e IGUAL-IGUAL-DIFERENTE aplicados a la detección de facturas fraudulentas en un conjunto de datos, permite encontrar casos que nos son fáciles de detectar mediante los métodos tradicionales de auditoría, como por ejemplo la selección de una muestra aleatoria al conjunto de datos, o muestreo estratificado o dada la experiencia de quien revise la información a criterio personal. Estas pruebas facilitan la selección de casos para investigar a fondo y verificar si lo que estos test detectaron corresponde a un error o son efectivamente casos de fraude de parte de las IPS.

▪	Con la aplicación del método IGUAL - IGUAL - DIFERENTE se identificó que algunas IPS radican la misma factura en los dos regímenes dejándolas en estados radicado activo, lo que implica una mala práctica por parte de las IPS. Se sugiere realizar un análisis detallado sobre estos casos para identificar si se trata de fraudes reales. Estos casos verificados corresponden al período de prestación de servicios del año 2020 en el cual se pudieron identificar mediante el método IGUAL-IGUAL-IGUAL 680 facturas por un valor total de $1.693.940.668,00  pesos M/CTE, El test IGUAL-IGUAL-DIFERENTE identificó 710 facturas por un valor de $2.677.555.382,00 pesos M/CTE y cabe resaltar de este test que en la teoría del profesor Nigrini se hace más eficiente entre mayor es el periodo de evaluación, si se expande el periodo de análisis a un año, queda la inquietud de cuántos casos se pueden encontrar, y hacer un análisis de comportamiento de las regiones año a año, y sobre todo cuantificar cuántos de estos casos fueron identificados en el proceso de auditoría tradicional. 

▪	Los rangos intercuartílicos permitieron identificar límites inferiores y superiores para cada servicio y de esta forma identificar los valores que estén fuera de este rango que se catalogaron como valores atípicos. Se identificaron 312.966 registros que junto con los test IGUAL-IGUAL-IGUAL e IGUAL-IGUAL-DIFERENTE fueron el punto de partida para la aplicación de modelos de clasificación supervisados.

▪	El algoritmo Random Forest tuvo la mayor precisión de todos los modelos utilizados, un  93%. Este modelo fue el que mejor pudo clasificar las facturas marcadas como sospechosas con un f1-score del 77% y del 96% a las facturas consideradas como normales. La explicación se debe a que este proyecto se basó en la identificación de datos atípicos dentro de la base de datos, y este tipo de algoritmo se caracteriza por realizar la clasificación basado en la búsqueda de datos atípicos. Con lo anterior podemos concluir que este modelo clasifica e identifica facturas sospechosas dentro de la base de datos de esta EPS. Si tenemos en cuenta la justificación de este proyecto que en el 2019 según reporte de la Supersalud las utilidades de las IPS aumentaron mientras que para el mismo periodo las pérdidas de las EPS se incrementaron. Este modelo puede funcionar como soporte al área de auditoría de la EPS que por volumen de facturación (8.561.061 registros que consta esta base para el 2020), les resulta casi imposible poder detectar y revisar estos errores en la facturación presentada por las IPS, siendo este modelo una alternativa para mejorar la identificación de fraudes en la facturación. 
