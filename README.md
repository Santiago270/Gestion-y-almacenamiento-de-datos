
# Base de datos: breast-cancer

En este proyecto se utiliza la base de datos breast-cancer.data, la cual fue obtenida del Centro Médico Universitario, Instituto de Oncología, Ljubljana, Yugoslavia. Agradecemos a M. Zwitter y M. Soklic por proporcionar los datos. 

## Problematica 
Considerando que para el año 2020 se registraron 2,3 millones de casos nuevos de cáncer de seno en mujeres a nivel mundial ”
-Organización Mundial de la Salud, 2023.
y teniendo en cuenta la informacion obtenida de la base de datos, se econtró que hay carencia de informacion precisa sobre la evolución del cáncer de seno en diferentes grupos de pacientes. 
## Contenido 
1. Base de datos sin proceso de limpieza (breast-cancer)
2. Base de datos limpia (Proyecto_Gestion_BD)
3. Codigo para la limpieza de la base de datos (Limpieza_de_datos.ipynb) 
* Instalaciones de librerias necesarias e importacion del data set.
* Visualizacion de la informacion del data set 
* Creeacion de la copia del dataset
* Datos repetidos
* Comteo de datos nulos 
* Limpieza de datos categoricos
* Grafico de caja para visualizacion de datos atipicos (variable numerica)
* Graficos comparativos con la variable objetivo ( deg_malig)
4. Codigo para implementacion de funciones y manipulacion de base de datos en MySql (Manipulación_de_datos.ipynb)
* Intalacion e importacion de librerias
* Creacion de la base de datos 
* Creacion de tabla
* Envio de data frame a BD MySql
*  Comprobacion de subida del data frame 
* Creacion de graficos a partir de los datos traidos de la BD
* Consultas SQL (CRUD) para simular la manipulación de la base de datos

## BD breast-cancer
### Tipo de datos de cada caracteristica:
* **Class** (object) \
* **age** (object)\
* **menopause** (object)\
* **tumor-size** (object)\
* **inv-nodes** object()\
* **node-caps** (object)\
* **deg-malig** (int)\
* **breast** (object)\
* **breast-quad** (object)\
* **irradiat** (object)\
### Caracteristicas: 
![Texto alternativo](caracteristicas.png)

## Conclusiones 

La identificación de características que puedan prever el grado de malignidad en el cáncer de mama es crucial para una detección y tratamiento efectivos. Según los datos disponibles, ciertos factores destacan como indicadores potenciales:

Primero, la combinación de tamaño del tumor y edad emerge como un predictor clave. Pacientes con tumores de 25-29 mm y edades entre 30 y 69 años tienden a ser diagnosticados con grados de malignidad más altos. Es importante destacar que las personas más jóvenes, especialmente entre 20 y 29 años, muestran una menor propensión a desarrollar tumores malignos según esta base de datos.

Además, la relación entre el grado de malignidad y la recurrencia del cáncer de mama es notable. Aquellos que experimentan recaídas tienden a presentar un grado de malignidad 3 con mayor frecuencia, mientras que aquellos sin recaídas suelen tener un grado de malignidad 2 predominante.

Un análisis más detallado revela que más de 20 individuos con cáncer de mama exhiben tumores de 30 a 34 mm y una edad promedio entre 50 y 52 años. Sin embargo, casos extremos, con tumores muy pequeños o grandes, son menos comunes y generalmente se asocian con una edad promedio más avanzada.

Asimismo, la ubicación del tumor dentro del seno podría influir en el grado de malignidad. Se observa un mayor porcentaje de casos con grado de malignidad 3 en pacientes con cáncer de mama en el seno izquierdo, lo que sugiere una posible variación en la agresividad del cáncer según la ubicación.

Estos hallazgos resaltan la importancia de considerar múltiples factores al evaluar el grado de malignidad en el cáncer de mama, lo que puede contribuir a una mejor comprensión del pronóstico y una atención más personalizada para los pacientes. Sin embargo, se necesitan más investigaciones para confirmar y ampliar estos patrones observados en la base de datos proporcionada.

Estas características identificadas pueden tener un impacto significativo en el desarrollo de estrategias de tratamiento personalizado para pacientes con cáncer de mama. Aquí hay algunas formas en que cada característica podría influir en dichas estrategias:

Tamaño del tumor y edad:

Pacientes con tumores más grandes y edades avanzadas pueden requerir enfoques de tratamiento más agresivos, como cirugía radical o quimioterapia intensiva, para abordar la enfermedad en sus etapas avanzadas.
Por el contrario, pacientes más jóvenes con tumores más pequeños pueden ser candidatos para opciones de tratamiento menos invasivas, como la terapia hormonal o la terapia dirigida, que pueden preservar la calidad de vida y la función mamaria.
Recurrencia y grado de malignidad:

Los pacientes que experimentan recurrencia y presentan un grado de malignidad 3 pueden beneficiarse de un seguimiento más riguroso y una terapia adyuvante más intensiva para prevenir la reaparición del cáncer.
Aquellos sin recurrencia pero con un grado de malignidad 2 pueden ser monitoreados de cerca, pero podrían beneficiarse de un enfoque de tratamiento más conservador para minimizar los efectos secundarios.
Ubicación del tumor:

La localización del tumor dentro del seno puede influir en las opciones de tratamiento. Por ejemplo, tumores en áreas cercanas al pezón pueden requerir técnicas quirúrgicas específicas para preservar la función mamaria y la estética.
La presencia de un mayor porcentaje de casos con grado de malignidad 3 en el seno izquierdo podría motivar una monitorización más intensiva o una evaluación más minuciosa de los ganglios linfáticos axilares en ese lado.
Tamaño del tumor y edad en un grupo específico:

Los pacientes con tumores de tamaño medio y edades promedio específicas pueden requerir un enfoque de tratamiento adaptado a sus necesidades y características individuales.
Las terapias combinadas o secuenciales podrían ser más apropiadas para este grupo, teniendo en cuenta la edad y la tolerancia al tratamiento.


## Valor generado para empresas

El análisis de las características del cáncer de mama y su relación con el grado de malignidad puede proporcionar varios beneficios empresariales, especialmente en el campo de la atención médica y la investigación oncológica. Algunos de estos beneficios incluyen:

Desarrollo de tratamientos personalizados: Comprender cómo diferentes factores influyen en el grado de malignidad del cáncer de mama puede impulsar el desarrollo de tratamientos más específicos y efectivos. Las empresas farmacéuticas y de biotecnología podrían aprovechar estos datos para desarrollar terapias dirigidas que aborden las características específicas de cada paciente, lo que podría conducir a mejores resultados clínicos y, potencialmente, a un aumento en la demanda de estos tratamientos.

Optimización de la atención médica: Las instituciones de salud pueden utilizar estos datos para mejorar la precisión diagnóstica y el manejo de pacientes con cáncer de mama. Esto podría resultar en una atención más eficiente y centrada en el paciente, lo que podría traducirse en una mayor satisfacción del paciente y una reputación mejorada para la institución médica.

Investigación y desarrollo de nuevas tecnologías: El análisis de datos sobre el cáncer de mama podría impulsar la investigación y el desarrollo de nuevas tecnologías, como biomarcadores específicos, métodos de detección temprana más precisos o herramientas de imagen avanzadas. Las empresas que desarrollen estas tecnologías podrían obtener ventajas competitivas significativas en el mercado al ofrecer soluciones innovadoras que mejoren el pronóstico y el tratamiento del cáncer de mama.

Consultoría y servicios especializados: Las empresas de consultoría en salud y análisis de datos podrían ofrecer servicios especializados en análisis de datos oncológicos y asesoramiento estratégico basado en estos análisis. Esto podría incluir la identificación de tendencias, el desarrollo de modelos predictivos para el pronóstico del cáncer de mama y la optimización de los protocolos de tratamiento en instituciones médicas.

Colaboración y asociaciones: El análisis de datos sobre el cáncer de mama podría facilitar la colaboración entre empresas, instituciones académicas y organizaciones de investigación. Esto podría conducir a asociaciones estratégicas para el desarrollo conjunto de terapias, tecnologías y programas de investigación, lo que beneficiaría a todas las partes involucradas y podría acelerar la innovación en el campo del cáncer de mama.


## Authors

- [@santiago270](https://github.com/Santiago270)

- [@1234manuela3](https://www.github.com/1234manuela3)

- [@isarodriguezv](https://www.github.com/isarodriguezv)