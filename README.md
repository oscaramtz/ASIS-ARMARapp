Objetivo del aplicativo
Servir de referente para la estandarización de análisis situacionales de salud para regiones territoriales en las américas.
Motivo y necesidades del aplicativo
Como te comentamos anteriormente, El ASIS un proceso analítico-sintético que permite “caracterizar, medir y explicar el perfil de salud-enfermedad de una población incluyendo los daños y problemas de salud, así como sus determinantes, sean estos competencia del sector salud o de otros sectores. Los ASIS facilitan la identificación de necesidades y prioridades en salud, así como la identificación de intervenciones y programas apropiados y la evaluación de su impacto en salud”

Para llevar a cabo su elaboración, recopilación de datos y el análisis se proponen las siguientes 7 líneas estratégicas:

1.	Contexto histórico, social, cultural y demográfico
2.	Analizar la salud, daños y riesgos a la salud
3.	Políticas, programas y servicios de salud
4.	Desigualdades en salud
5.	Prioridades en salud
6.	Evaluación
7.	Participación social y abogacía
Los puntos señalados en amarillo son los que se buscan sistematizar para agilizar el reporte de un ASIS.
Productos esperados y diseño del aplicativo o página web
1.	Guía para la elaboración del ASIS
En este rubro se busca realizar un tipo WIKI tipo step-by-step, que sea dinámico para guiar a los usuarios a la realización y los factores a tomar en cuenta de un Análisis Situacional en Salud (Dicho manual ya existe, pero en extenso en un documento de 90 páginas y varios manuales).
Para fines prácticos los “capítulos” (por llamarlos de alguna manera) son 7
1.	Prefacio
2.	Introducción y antecedentes
3.	Sección I Definición de ASIS ARMAR-7 y factores a considerar para su realización
4.	Sección II La planeación del ASIS
5.	Sección III Fases ARMAR
a.	Articulación
b.	Recopilación de información
c.	Manejo de información
d.	Análisis de información
e.	Reporte
6.	Sección IV Componentes estratégicos del ASIS
a.	Contexto histórico, social, cultural y demográfico
b.	Analizar la salud, daños y riesgos a la salud
c.	Políticas, programas y servicios de salud
d.	Desigualdades en salud
e.	Prioridades en salud
f.	Evaluación
g.	Participación social y abogacía
h.	Pasos para el desarrollo del ASIS ARMAR
7.	Bibliografía y otros documentos de consulta
Presentar la estructura del Wiki de manera dinámica con un SIDEBAR desplegable con acción (un toggle) y con imágenes de ejemplo, tipo el intro.js que me mostraste step-by-step para que sea dinámico

2.	Plantillas de captura, procesamiento de datos y plantillas de análisis
Esta segunda parte del producto es más como lo platicamos el viernes 6 de octubre, para fines de facilitar el análisis nosotros proponemos por una parte tener datos precargados, que son las bases de datos que te comento (Ej. INEGI microdatos*, SSA datos abiertos*, Recursos en salud, entre otros, Cubos dinámicos de la DGIS, bases de datos del Banco Mundial) para que sean procesadas por la misma app o sitio web y que este arroje información y gráficos suficientes para realizar el análisis.
Para lo cual, se espera que los usuarios que quieran hacer uso de la plataforma se loguen para guardar datos.
Para esto se busca procesarlos de la siguiente manera, retomando los 7 componentes del ASIS:
1.	Contexto histórico, social, cultural y demográfico
2.	Analizar la salud, daños y riesgos a la salud
3.	Políticas, programas y servicios de salud
4.	Desigualdades en salud
5.	Prioridades 
6.	Evaluación
7.	Participación social y abogacía
8.	Pasos para el desarrollo del ASIS ARMAR
Por otro lado, desde el componente 1 al componente 4 se necesita tener una línea de captura que permita capturar en cualquier punto mientras el usuario navega por los distintos componentes, al identificar un problema en particular (por ejemplo, al ver la información de un municipio y desagregarla por localidades viendo el menor y el mayor y sus diferencias, identifica que el municipio “X” tiene altos niveles de pobreza alimentaria) pueda capturar en una línea de texto “El municipio “X” tiene mayores índices de pobreza”; esto con la finalidad de ser utilizado posteriormente para la priorización (componente 5)

En el primer componente (Contexto histórico, social, cultural y demográfico) se necesitan datos sobre características de la población
-	¿Cuánta población existe en México por municipios, estados, nacional, divididas por edad o por grupos de edad?
-	¿Cuál es su dinámica poblacional, en cuanto a que escolaridad tienen, su ingreso bruto percapita, etc?
-	Y poder graficar dichos datos
-	Ejemplo.- Datos demográficos Tableau Dashboards
-	Otro ejemplo.- Datos demográficos PowerBI de MS
En el segundo componente (Analizar la salud, daños y riesgos a la salud) para este componente se requieren datos sobre daños de la salud, cuantas personas se enferman de una región en particular, cuantas personas mueren de una región en particular. 
-	El punto crucial en este rubro es manejar el modelo de base de datos que, al igual que en el componente demográfico, te permita manipular el “cuantos” mediante filtros de características particulares, por ejemplo: cuantos menores de 5 años enferman de vías digestivas, cuantas mujeres mayores de 20 años enferman de cáncer, cuantos hombres mayores de 65 años mueren por secuelas de enfermedades cardiovasculares. 
-	Para todas estas particularidades existen las bases de datos y los catálogos de clasificación de enfermedades y mortalidad.
-	Cuantos menores de 5 años son vacunados, cuantos no etc.
-	Ejemplo.- Resultados en salud, Tableau Dashboards
-	Ejemplo.- Mortalidad VizHub de IHME
-	Ejemplo.- Carga de la enfermedad VizHub de IHME
-	Ejemplo.- Mortalidad VizHub de IHME
El tercer componente (Políticas, programas y servicios de salud) es muy similar, para este rubro existe una base de datos con catalogos que permiten conocer con cuantos recursos en salud cuenta cada localidad de la nación (cuantos consultorios, cuantos médicos generales, cuantos especialistas, cuantas enfermeras, nutriólogos, etc)
-	Ejemplo.- Consulta a Mujeres en edad reproductiva Tableau Dashboards (varias pestañas)
Y después los componentes cuarto y quinto que demandan mayor procesamiento.
En el cuarto (Desigualdades en salud) este componente es un poco más complejo, para este componente se obliga la identificación de indicadores por la totalidad de municipios de un estado o la totalidad de localidades de un estado, ya que para este componente existen fórmulas para las métricas en desigualdades que son simples y otras complejas. Pero todas ya están bien clasificadas y para qué sirven cada una de ellas.
El punto crucial de estas métricas de desigualdades en salud es que puedas identificar qué población separada o filtrada por características demográficas son más desiguales que otra población un ejemplo sencillo sería:
La población de Xochimilco tiene una tasa específica de escolaridad en el grupo de 15 a 24 años menor que la población de ese mismo grupo de edad en Miguel Hidalgo, al comparar las tasas de embarazo adolescente existe mayor cantidad de población en Xochimilco que en Miguel Hidalgo. Este resultado en salud puede ser explicado con las características particulares de población.
En el Quinto componente (Prioridades), se espera que el usuario pueda utilizar de manera práctica distintas metodologías de priorización, pero en particular el Índice de necesidades en salud. Para lo cual es necesario que, de los indicadores vistos en el componente Demográfico, de resultados en salud, recursos en salud métricas de desigualdad, se puedan arrastrar para priorizar regiones territoriales mediante la aplicación.
Anexo documento con fórmulas Excel para que quede más claro para que quede más claro.
3.	Apoyo con la redacción
El objetivo principal de este rubro es que al tiempo que se navega por los componentes anteriores, se puedan elegir una serie de tablas de salida, gráficos e imágenes para la realización de un reporte, dentro de este producto se espera que el usuario registrado que haya guardado sus tablas, indicadores importantes , gráficas o imágenes, se le apoye con la redacción del reporte mediante una plantilla Word o tipo Word con un tipo intro.js o step-by-step guide, para guiar al usuario con la redacción del reporte final, esto mediante una serie de preguntas que ya se tienen establecidas para cada uno de los rubros.
# ASIS-ARMARapp
Aplicativo ASIS ARMAR-7
