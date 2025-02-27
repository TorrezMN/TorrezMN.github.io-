# Optimización de Costos de Producción: Estrategias y Análisis de Datos en una Empresa Electrónica
AnálisisDeDatos ,OptimizaciónDeProducción ,GestiónDeInventarios ,EstrategiasDeMejora

<div style="text-align: center; margin-top: 50px; background-color: gray;
padding: 20px; ">


Este desafío es una oportunidad crítica para demostrar habilidades analíticas
en el contexto de una postulación para un puesto de analista de datos. Se trata
de abordar un problema real relacionado con la optimización de costos de
producción en una empresa de fabricación de dispositivos electrónicos,
analizando datos históricos y proponiendo mejoras estratégicas. La capacidad
para analizar y interpretar datos, verificar su integridad y aplicar soluciones
efectivas en un entorno teórico es esencial para destacar en el proceso de
selección. Este desafío no solo permite evaluar competencias técnicas, sino
también la habilidad para abordar problemas complejos y presentar soluciones
prácticas y bien fundamentadas.


Este es mi abordaje personal para el desafío. Presento mi estrategia de de
trabajo para afrontar el desafío. 

Se asume que todo el planteamiento es netamente teórico. Por esta razón pueden
existir aspectos faltantes que en escenarios reales deben analizarse o
mejorarse. Por ej. la calidad de los datos disponibles como así también el tipo
de datos por ej. cajas de papel vs tablas en bases de datos.

</div>





# DESCRIPCIÓN DEL PROBLEMA 

---



Imagina que has sido contratado como Analista de Datos en una **empresa de
fabricación de dispositivos electrónicos**. Antes de tu reunión inicial con el
equipo directivo, te ofrecen un recorrido por la planta de la mano del jefe de
turno.

El recorrido comienza en el ***depósito de materias primas***. Caminas por
pasillos llenos de *materiales apilados hasta el techo en algunas secciones,
mientras que otras áreas están completamente vacías*. El jefe de turno comenta:
"Hemos recibido una gran cantidad de componentes esta semana, pero parece que
**nos hemos quedado cortos de algunos insumos cruciales**."

Luego pasas a la ***sala de producción***, donde observas varias líneas de
producción idénticas. De las diez líneas que ves, cinco funcionan de manera
fluida y eficiente, con operarios trabajando sincronizadamente. En las otras
cinco, la situación es diferente. Dos líneas tienen productos acumulados en
varios puntos. *En una línea, los operarios están parados junto a máquinas
detenidas, esperando a que se reanuden*. Escuchas a un operario decir: "**Otra
vez se detuvo la máquina.** Necesitamos que venga el técnico de mantenimiento."
Otro operario responde: "Sí, **ha estado fallando toda la semana.** Esto nos
está retrasando mucho." Las otras dos líneas más están completamente paradas,
sin operarios a la vista.

La siguiente parada es el ***depósito de productos terminados***. Aquí, ves
*espacios de bodega densamente cargados y otros espacios donde faltan
productos*. Escuchas a un empleado diciendo: "**Otra vez nos quedamos sin poder
completar el cargamento** de protectores de sobrecargas." Otro empleado
responde: "aunque no sobren, al menos, los **circuitos temporizadores nunca
faltan**" Mientras continúas, otro trabajador menciona: "Tenemos que reubicar
las placas de control, están ocupando demasiado espacio."

Después del recorrido, llegas a la reunión con el equipo directivo. Ellos te
explican que tu primer proyecto esta relacionado con la optimización los costos
de producción. Te proporcionan acceso a una vasta cantidad de datos históricos
que incluyen registros de producción, inventarios, costos de materia prima,
entre otros. Tu trabajo inicial implica verificar la integridad y veracidad de
estos datos, proponer mejoras en la gestión de adquisición y registro de datos,
para luego identificar áreas de mejora y optimización.


## **OBJETIVOS DEL PROYECTO**

1- Optimización de costos de producción.

2- Verificar la integridad y veracidad de datos.

3- Proponer mejoras en la adquisición y registro de datos.

4- Identificar áreas de mejora y optimización.


### Observaciones sobre los objetivos del proyecto. 

Dado que el presente es un ejercicio teórico solo se puede especular sobre los
posibles resultados del mismo. Únicamente se presentan posibles caminos a
seguir.

Sobre la *integridad y veracidad de los datos.* **no se provee mayor claridad
sobre los métodos de recolección de datos** actuales y datos disponibles para
análisis.

Sobre las *mejoras en la adquisición y registro de datos.* Una vez finalizado
el proyecto se pueden establecer criterios de validación y recolección de
datos, según utilidad características, prioridades y necesidades. 

Sobre *identificar áreas de mejora y optimización.* Tanto en los procesos de
producir como así también los procesos de recolección y validación de datos.
Solo es posible proveer sugerencias para mejoras una vez culminada la
investigación. 


## DATOS/HERRAMIENTAS

Inicialmente se tiene a disposición, para el desarrollo del proyecto, los
siguientes datos.

- Datos históricos.
    - Registros de producción.
    - Inventarios
    - Costos de materia prima.

- Stack de herramientas.
    - python
    - pandas
    - matplotlib
    - seaborn
    - jupyter notebooks


<a id="datos_de_interes"></a> 

## DATOS DE INTERÉS 


---

Se mencionan a continuación los datos que serian de interés para el proyecto.
Datos necesarios como así también información de utilidad para el proyecto.

* **MATERIAS PRIMAS**   
     - Oferta de materias primas y costos.   
     - Costos de almacenamiento.
     - Normativas de uso internacionales. (Implica algún costo adicional su
       utilización?)
 
* **PRODUCCIÓN**
     - Operarios involucrados en producción y mantenimiento.
     - Productividad de cuadrillas de operarios. (Operarios involucrados,
       tiempo en la empresa vs. productividad.)
     - Historial de mantenimiento.
     - Cronograma de mantenimiento.
     - Costos de mantenimiento.
     - Costos de inactividad. 
     - Rentabilidad de productos terminados vs materia prima.
     - Cumplimiento de normas internacionales para la producción. (Se deben
       cumplir normas internacionales para la producción?. Tipo certificaciones
       internacionales. permisos ambientales, etc.)
     - Tiempos de producción vs. costo por producto.
     - Tiempos de producción vs. costo por cuadrilla de operarios.
 
* **PRODUCTOS TERMINADOS**
     - Costo de almacenamiento.
     - "Completar cargamentos".  
     - Valuación temporal del producto. (Varia su valor según el tiempo que
       pasa en almacén?)
     - Ubicación de productos?.

## ESTRATEGIAS DE ANÁLISIS 

---

Se describe a continuación las estrategias de desarrollo y análisis del
proyecto. Que tipo de análisis se utilizaría. Las herramientas que se
utilizarían. 


### OBSERVACIONES INICIALES 

Para realizar la investigación se aria una segmentación en áreas de interés
según lo indicado en los párrafos anteriores: *materias primas, producción,
productos terminados*.

Dado que no se puede evaluar del desempeño productivo de una empresa
considerando únicamente factores internos. Para el proyecto inicial se
procedería con un análisis exhaustivo de los datos iniciando con los últimos 10
años previos al inicio del proyecto. Últimos 10 años en periodos de 2 años.
Esto es 5 periodos de 2 años cada uno. 

*Una vez culminado el proyecto inicial se pueden reducir los periodos
temporales para proyectos futuros.*    
   

Esto es porque:

- Fiestas nacionales. En algunas ocasiones el gobierno dictamina feriados
  nacionales en memoria de algún evento especial. 

-  Las regulaciones gubernamentales cambian. Permitiendo o restringiendo
   importaciones. Imponiendo variaciones impositivas. etc.

-  Existen periodos de inactividad obligatoria como la [pandemia
   covid-19](https://es.wikipedia.org/wiki/Pandemia_de_COVID-19) ocurrida en el
   año 2020-2023 que afecto la producción y economía mundial.

-  Existen competencias económicas o sanciones impuestas entre gobiernos que
   hacen que la economía y la producción varié.

-  En algunas ocasiones las temporadas de invierno son mas fuertes que en otras
   provocando de esta forma que los operarios sufran mas enfermedades de época.

Estas son solo algunas de las razones existentes que hacen necesaria la
segmentación temporal en el proceso de análisis para poder evaluar de forma
individual y veraz los datos existentes.

<a id='proc_por_area_de_interes'></a>

### Procedimientos para cada área de interés. 


El procedimiento para realizar el análisis en cada área de interés. Seria el
siguiente:

- Obtención de datos mediante consultas sql u otro tipo de métodos.

- Se realizaran tareas de limpieza de datos y normalización de datos.

- Se realizaran tareas exploratorias de datos. Teniendo en cuenta lo expuesto
  en el apartado [DATOS DE INTERÉS](#datos_de_interes).

- [**ANÁLISIS DE
  Pareto**](https://es.wikipedia.org/wiki/Principio_de_Pareto).[^2]
[^2]: Es un postulado que establece de manera arbitraria que el el 80% de los
efectos proviene del 20% de las causas. Podría traducirse en términos
empresariales: *es probable que el 20% de los clientes generen aproximadamente
el 80% de los ingresos de una empresa.*  para cada área de interés dentro del
análisis se intentaría identificar los factores de éxito para la optimización
de los procesos de la empresa.

- Para cada caso se intentara identificar los factores de mayor productividad
  que son de interés según lo expuesto en el apartado [DATOS DE
  ITERES](#datos_de_interes). 

- Análisis global del proyecto. una vez finalizadas las etapas anteriores y con
  una visión mas amplia de los procesos de la empresa. Se procede a realizar
  una integración global de los resultados. Redactando conclusiones para cada
  área de interés del proyecto.

- conclusiones finales. Integración de conclusiones finales en una conclusión
  final del proyecto indicando hallazgos principales y puntos fuertes y débiles
  del proceso de producción.

**PRESENTACIÓN DE RESULTADOS**   

---

La metodología de presentación de los resultados seria a través de informes
ejecutivos. No mas de 5 paginas por área de interés resaltando los hallazgos, los
puntos fuertes y débiles con respecto al área analizadas incluyendo gráficas
para ilustrar los datos de mayor relevancia.

En cuanto a "gráficas ilustrativas" se limitara al uso de gráficos de barra y
gráficos de torta en lo posible. Dado que son muy comunes y fáciles de
interpretar.

Se anticipa también la elaboración de "tableros" con herramientas que permitan el
acceso 24/7 a la información existente permitiendo de esta forma que los
ejecutivos puedan acceder a la misma cuando sea necesario. Con herramientas
tales como: plotly-dash, panel, streamlit, etc.


### INCÓGNITAS INICIALES

A modo "trabajo inicial" se procede a establecer parámetros iniciales de
comparación para cada una de las categorías expresadas en los párrafos
anteriores. [DATOS DE INTERÉS](#datos_de_interes).

Esta tarea provee parámetros de comparación iniciales para evaluar
posteriormente el desempeño de las "mejoras" aplicadas.

Se exponen algunas "incógnitas" que sirven de puntapié inicial para el análisis
de los datos proveídos por la empresa.

* **MATERIAS PRIMAS**   

     - Cual es la oferta de materias primas? Cuantos proveedores hay? Tiempos
       de entrega. 
     - La empresa tiene bodegas propias? Se alquilan? Costos de alquiler.
     - Existen normativas que regulen la producción? Se necesita habilitación?
       Las habilitaciones por cuanto tiempo tienen vigencia?
     - Implican algún costo adicional las habilitaciones?
 
* **PRODUCCIÓN**

     - Desempeño de operarios.
         - Horas trabajadas.
         - Faltas
         - Cumplimiento de tareas.
     - Cuadrillas de operarios.
         - Como se crean las cuadrillas de operarios? Se eligen al azar? Se
           asignan "manualmente"?
         - Identificar cuadrillas mas productivas. Identificar factores que
           hacen a la productividad. Son operarios con mucho tiempo en la
           empresa o poco tiempo. producen en función del salario recibido.
     - mantenimiento
         - Existen calendarios de mantenimiento?
         - Motivos por los cuales hay maquinas paradas.
         - Historial de mantenimiento.
         - proveedores de repuestos y costos de mantenimiento.
         - Costos por inactividad de maquinas y operarios.
     - Costos de producción vs. materia prima y cadena de suministros.
     - Normativas internacionales.
         - Costos de certificaciones.
         - Costos de habilitaciones.
         - Permisos de trabajo por factores ambientales.
     - Tiempos de producción.
         - Tiempos de producción vs. costos por producto.
         - Tiempos de producción vs. costos por cuadrillas de operarios.

 
* **PRODUCTOS TERMINADOS**

     - Cuanto cuesta tener los productos almacenados en bodega? (Dinero perdido
       vs. tiempo perdido.)
     - Motivos por los que no es posible "completar cargamentos".
     - Valuación temporal del producto. (Varia su valor según el tiempo que
       pasa en almacén?)
     - Estrategias de locación de productos.


## **PARA FUTURAS PROYECTOS**      

---   

Una vez finalizado el proyecto y para el desarrollo de futuros proyectos.
Teniendo una visión mas amplia del funcionamiento de los procesos de la empresa
y dominio de negocio de la empresa. Se pueden establecer criterios de
automatización en la recolección de datos. 

A primera vista se pueden identificar dos aspectos a tener en cuenta: *aspectos
técnicos y aspectos teóricos/analíticos*.

- *Aspectos técnicos.* Este aspecto contempla todo lo relacionado a obtención y
  optimización de la recolección de datos. Contando con una evaluación mas
  detallada de los procesos de recolección se pueden proponer modificaciones
  para *garantizar la veracidad y utilidad de los datos* recolectados. Así
  también garantizar la disponibilidad de los mismos. En materia de
  "automatización" de procesos se pueden establecer puntos de interés como la
  recolección de datos y el proceso de "limpieza de datos" como puntos posibles
  a procesos de automatización.

- *Aspectos teórico/analíticos* contemplan todo lo relacionado al análisis de
  los datos. Metodologías de análisis de datos numéricos, temporales, etc. en
  la sección donde se detallan los [procedimientos para cada área de
  interés](#proc_por_area_de_interes) se menciona el "análisis pareto". ara
  nuevos proyectos se intentaría incorporar nuevos métodos de análisis que sean
  relevantes al campo de estudio y las necesidades del dominio de interés del
  proyecto. Se pueden optimizar también los periodos temporales de análisis de
  datos para el proyecto. Aumentar la temporalidad o reducirla.

Se puede evaluar también la implementación de sistemas de alerta o "modelos
predictivos" para escasez de stock de materia prima o sobre producción.
Permitiendo de esta forma estar preparados o minimizar de forma eficiente el
gasto de producción a futuro y maximizando las ganancias.
