# El ecosistema de Big Data 

Big Data no es solo un problema de base de datos o una herramienta en particular, es todo el complejo de componentes para almacenar, procesar, visualizar y entregar resultados a las aplicaciones de destino. Todo este complejo interrelacionado se puede definir como el ecosistema de Big Data que se ocupa de la evolución de los datos, los modelos y la infraestructura requerida durante todo el ciclo de vida de Big Data.

El ecosistema de Big Data es demasiado grande, complejo y redundante. Es un mercado confuso para las personas y empresas que han aceptado la idea del Big Data, pero luego tropiezan cuando se enfrentan a demasiadas decisiones en numerosas capas de la tecnología. Resulta sumamente difícil describir todas las tecnologías que componen el ecosistema de Big Data, es por esto que dichas tecnologías han sido divididas en diferentes categorías y estas a su vez se han llegado a dividir en áreas mas especificas. A continuación se definen algunas de las categorías y componentes más importantes que abordan los diferentes aspectos del ecosistema de Big Data:

---

## Tipos de datos

Las diferentes etapas de la transformación de Big Data requieren y utilizan diferentes estructuras de datos, modelos y formatos.

<br>

<p>
<img align="left" width="700" height="350" src="https://dtflaneur.files.wordpress.com/2013/02/svuns.png?w=700">
</p>


* **Datos estructurados**: Los datos estructurados se refieren a todos los datos que se pueden almacenar una base de datos relacional, en tablas con filas y columnas. Tienen una clave relacional y se pueden mapear fácilmente en campos prediseñados. La información estructurada es relativamente simple de ingresar, almacenar, consultar y analizar, pero debe estar estrictamente definida en términos de nombre y tipo de campo.

* **Datos no estructurados**: Los datos no estructurados pueden tener su propia estructura interna, pero no se ajustan perfectamente a una hoja de cálculo o base de datos. El desafío fundamental de las fuentes de datos no estructurados es que son difíciles de descifrar, comprender y preparar para el uso analítico.

* **Datos semiestructurados**: Los datos semiestructurados son información que no reside en una base de datos relacional pero que tiene algunas propiedades organizacionales que hacen que sea más fácil de analizar. Por ejemplo los archivos CSV, XML y JSON son documentos semiestructurados y las bases de datos NoSQL se consideran semiestructuradas.

<br>

---

### Bases de datos

<br>

<p align="center">
<img  src="https://blog.couchbase.com/wp-content/uploads/2017/04/nosql-vs-sql-overview-1.png">
</p>

* **Bases de datos relacionales**: Bases de datos operacionales para aplicaciones OLTP que requieren altas cargas de transacciones y concurrencia del usuario. Puede "ampliarse" a volúmenes de datos, pero no tiene la capacidad de "escalar horizontalmente" para el procesamiento de datos de gran tamaño. Poseen un esquema estructurado de tablas que contienen filas y columnas de datos que enfatizan la integridad y la coherencia sobre la velocidad y la escala. Datos estructurados a los que se accede con el lenguaje de consulta SQL. Algunas de las más populares son SQL Server, Oracle, MySQL , PostGreSQL, IBM DB2.

* **Base de datos analíticas**: Esquema estructurado de tablas que contiene filas y columnas de datos que ofrecen velocidad y escalabilidad mejoradas en RDBMS, pero que aún se limitan a datos estructurados. Los esquemas rígidos con consultas SQL orientadas a lotes no están diseñados para aplicaciones de streaming. Algunas de las más populares son Oracle Exadata, IBM Netezza, EMC Greenplum, Vertica.

* **Bases de datos NoSQL**: Bueno para aplicaciones web, código de aplicación web sin escritura, depuración y mantenimiento. Escale el escalado horizontal con datos automáticos para admitir a millones de usuarios de aplicaciones web. Compromiso de coherencia (transacciones ACID) a favor de la escala y el tiempo de actividad. El diseño sin esquema permite una ingesta rápida o continua a escala. Buena opción de almacenamiento para alto rendimiento, bajos requisitos de latencia de aplicaciones de transmisión para vistas de datos en tiempo real. Visto como un componente clave de la arquitectura Lambda. Algunas de las más populares son: MongoDB, HBase, Cassandra, MarkLogic, Couchbase.

* **Bases de datos NewSQL**: Corresponde a un nuevo (relativamente) tipo de base de datos que se considera un nuevo paradigma de base de datos RDBMS, en el que se aplican las lecciones aprendidas de las bases de datos NoSQL en el mundo SQL. Están pensadas principalmente para aplicaciones que requieren gestionar gran cantidad de registros, pero con la consistencia que ofrecen las RDBMS y mediante lenguaje SQL. Con respecto a este tipo de bases de datos, hay dos variantes: las que se han creado desde el principio con este concepto (VoltDB, MemSQL, etc.) y las que se han adaptado a este requisito, como es el caso de MySQL Cluster. Algunas de las más populares son Altibase, c-treeACE, CockroachDB, NuoDB, VoltDB.

* **Bases de datos orientadas a grafos**: Una base de datos orientada a grafos (graph database) representa la información como nodos de un grafo y sus relaciones con las aristas del mismo, de manera que se pueda usar teoría de grafos para recorrer la base de datos ya que esta puede describir atributos de los nodos (entidades) y las aristas (relaciones). Algunas son ArangoDB, Graphbase, Neoj, AllegroGraph, entre otras.

* **Bases de datos MPP**: Una base de datos MPP (massively parallel processing) es una base de datos que está optimizada para procesarse en paralelo para que muchas unidades de procesamiento realicen muchas operaciones a la vez. Algunas son MemSQL, Teradata, Vertica, entre otras.

---

## Lenguajes de programación

<br>

<img  height="100" width="300" src="https://cdn-images-1.medium.com/max/1600/1*PPIp7twJJUknfohZqtL8pQ.png">

* **Python**: Python es un lenguaje de programación fácil de aprender, identifica y asocia automáticamente tipos de datos y sigue una estructura de anidamiento basada en indentación. Tiene su disposición una gran cantidad de librerías para trabajar con Big Data como PyDoop , PySpark, NumPy, Pandas, Scipy entre otras.


<img  height="100" width="300" src="https://www.scala-lang.org/resources/img/frontpage/scala-logo-white@2x.png">

* **Scala**: Scala combina programación orientada a objetos y funcional en un lenguaje conciso y de alto nivel. Los tipos estáticos de Scala ayudan a evitar errores en aplicaciones complejas, y sus tiempos de ejecución de JVM y JavaScript le permiten construir sistemas de alto rendimiento con fácil acceso a un enorme ecosistema de bibliotecas.

<img  height="100" width="140" src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/1b/R_logo.svg/724px-R_logo.svg.png">

* **R**: R es un entorno y lenguaje de programación con un enfoque al análisis estadístico. Se trata de uno de los lenguajes más utilizados en investigación por la comunidad estadística, siendo además muy popular en el campo de la minería de datos, la investigación biomédica, la bioinformática y las matemáticas financieras.

---
### Motores de ejecución

<br>

<img height="100" width="300" src="https://lh6.googleusercontent.com/XeINihIXJLU3b2TH6HsottOgPnyVljd0nsjbkFgxPVxa2Bu8gDntmPFJT6GlYTC1qDwOzQ3Zatdwhw=w1680-h944">

* **Apache Hadoop** : Es un framework de código abierto de Apache escrito en java que permite el procesamiento distribuido de grandes conjuntos de datos en grupos de computadores utilizando modelos de programación simples. Una aplicación que trabaja en Hadoop funciona en un entorno que proporciona almacenamiento distribuido y computación entre clusters de computadoras. Hadoop está diseñado para escalar desde un único servidor a miles de máquinas, cada una de las cuales ofrece cómputo y almacenamiento local. Los componentes principales de Hadoop son:

    * **HDFS** : Es un sistema de archivos distribuidos y tolerante a fallas, diseñado para convertir un grupo de servidores estándar en un grupo de almacenamiento de escalamiento masivo. Desarrollado específicamente para cargas de trabajo de procesamiento de datos a gran escala donde la escalabilidad, la flexibilidad y el rendimiento son críticos.
    
    * **MapReduce** : MapReduce es el corazón de Apache Hadoop. Es este paradigma de programación que permite una escalabilidad masiva en cientos o miles de servidores en un clúster de Hadoop, permite escribir fácilmente aplicaciones que procesan grandes cantidades de datos en paralelo en grandes clusters (miles de nodos) de hardware básico de una manera confiable y tolerante a fallas.
    
    * **YARN** : Es un framework para la programación de trabajos y la administración de recursos del clúster. Proporciona administración de recursos de código abierto para Hadoop, por lo que puede ir más allá del procesamiento por lotes y abrir sus datos a un conjunto diverso de cargas de trabajo, que incluyen SQL interactivo, modelado avanzado y transmisión en tiempo real.
    
<img  height="100" src="https://lh6.googleusercontent.com/W0ONjRetitE3LX6xWYoxd3eUK8apdT5A_H2CYCl6zyv6rC4BoLoag-Rvhv3YDabIQLd_7sUpz3akpg=w1680-h944">

* **Apache Tez**: Apache Tez es un framework extensible para la construcción de lotes de alto rendimiento y aplicaciones interactivas de procesamiento de datos, coordinado por YARN en Apache Hadoop. Tez mejora el paradigma MapReduce al mejorar drásticamente su velocidad, al tiempo que mantiene la capacidad de MapReduce para escalar a petabytes de datos.

<img  height="100" src="https://lh4.googleusercontent.com/ibBRAUkBuhKbZI_27Jdu8b0fGMVbnNgewqjRbjiW7qT1Y98gThLBpxFc6L8ed1ndkCTdE1OQQCV0EA=w1680-h944">

* **Apache Spark**: Es un motor rápido de procesamiento de datos en memoria con APIs de desarrollo elegantes y expresivas para permitir a los trabajadores de datos ejecutar de manera eficiente la transmisión, el aprendizaje automático o las cargas de trabajo SQL que requieren un acceso iterativo rápido a los conjuntos de datos. Con Spark funcionando en Apache Hadoop YARN, los desarrolladores de todo el mundo ahora pueden crear aplicaciones para explotar el poder de Spark, obtener ideas y enriquecer sus cargas de trabajo de ciencia de datos dentro de un solo conjunto de datos compartido en Hadoop.

<img  height="100" src="https://data-artisans.com/wp-content/uploads/2017/02/flink-logo-large.jpg">

* **Apache Flink**: Apache Flink (en alemán significa "rápido") es un framework de Big Data para el procesamiento de datos por lotes y en streaming. Permite a los desarrolladores construir pipelines de procesamiento de datos complejas y ejecutarlas en un entorno distribuido. Proporciona un soporte de primera clase para el procesamiento en streaming e implementa el procesamiento por lotes como un caso especial.

---

## Gestión de clusters

<br>

<img  height="100" width="200" src="http://errequeerre.es/wp-content/uploads/2017/09/hadoop-yarn-300x191.png">

* **Hadoop YARN**: Hadoop YARN, un framework informático distribuido para la programación de trabajos y gestión de recursos de clúster, tiene alta disponibilidad para masters y esclavos, soporte para contenedores Docker en modo no seguro, ejecutores de contenedores Linux y Windows en modo seguro y un programador conectable.


<img  height="100" width="300" src="https://opencredo.com/wp-content/uploads/2015/12/apache-mesos.png">

* **Apache Mesos**: Apache Mesos, un kernel de sistemas distribuidos, puede administrar recursos por aplicación y tiene soporte para contenedores Docker. Puede ejecutar trabajos Spark, Hadoop MapReduce o cualquier otra aplicación de servicio. Tiene API para Java, Python y C ++.

<img  height="250" width="400" src="https://sharebigdata.files.wordpress.com/2016/01/clustermode.png">

* **Spark Standalone**: El administrador de clúster Spark Standalone es un administrador de clúster simple disponible como parte de la distribución de Spark. Es resistente a las fallas de los workes nodes, tiene capacidades para administrar recursos por aplicación, y se puede ejecutar junto con una implementación de Hadoop existente y acceder a los datos de HDFS.


---

## Streaming

<br>

<img  height="100" width="300" src="https://lh3.googleusercontent.com/CgQNPQ6S2O_9k-Ag45VSe3l8rYQ1a8cGd8kjzMAyYryNSpu3Fx_zw2ju5j1qICpq6BXopRH-_O0IVw=w1680-h944">

* **Apache Storm**: Apache Storm es un sistema de computación distribuido, tolerante a fallas y de código abierto. Storm procesa flujos de datos en tiempo real con Hadoop. Las soluciones de Storm también pueden proporcionar un procesamiento de datos garantizado, con la capacidad de reproducir datos que no se procesaron correctamente la primera vez.

<img  height="100" width="300" src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/ff/Apache-nifi-logo.svg/512px-Apache-nifi-logo.svg.png">

* **Apache Nifi**: Apache NiFi es una plataforma integrada de logística de datos para automatizar el movimiento de datos entre sistemas dispares. Proporciona control en tiempo real que facilita la gestión del movimiento de datos entre cualquier fuente y cualquier destino.

<img  height="100" width="300" src="https://i1.wp.com/www.clubdetecnologia.net/wp-content/uploads/2017/11/apache-kafka.png?resize=768%2C193">

* **Apache Kafka**: Apache Kafka es una plataforma de transmisión distribuida capaz de manejar billones de eventos al día. Inicialmente concebido como una cola de mensajes, Kafka se basa en una abstracción de un registro de compromiso distribuido.

---

## Machine Learning

<br>

<img  height="150" width="200" src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/11/TensorFlowLogo.svg/348px-TensorFlowLogo.svg.png">

* **TensorFlow**: TensorFlow es una biblioteca de código abierto que se basa en un sistema de redes neuronales. Esto significa que puede relacionar varios datos en red simultáneamente, de la misma forma que lo hace el cerebro humano. Por ejemplo, puede reconocer varias palabras del alfabeto porque relaciona las letras y fonemas.

<img  height="100" width="200" src="https://stradata.co/wp-content/uploads/2017/02/Mahout.jpg">

* **Mahout**: Apache Mahout es un proyecto de la Apache Software Foundation para producir implementaciones gratuitas de algoritmos de aprendizaje automático distribuidos o escalables, enfocados principalmente en las áreas de filtrado colaborativo, clustering y clasificación. Muchas de las implementaciones usan la plataforma Apache Hadoop.

<img  height="100" width="300" src="https://www.woodmark.de/blog/wp-content/uploads/2017/09/Spark-vs-flink-300x85.jpg">

* **Spark & Flink**: Spark tiene su propia libreria de aprendizaje automático,la cual es, MLlib. Los algoritmos de aprendizaje automático son muy rápidos, eficientes y optimizados en Spark gracias a la computación en memoria. Flink tiene la FlinkML, que es la libreria de Machine Learning para Flink. Los algoritmos de aprendizaje automático son muy rápidos, eficientes y optimizados en Flink debido a su soporte nativo para el procesamiento iterativo y la computación en memoria.

---

## Big data como servicio

<br>

<img  height="100" width="200" src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/1d/AmazonWebservices_Logo.svg/580px-AmazonWebservices_Logo.svg.png">

* **AWS**: Amazon Web Services (AWS) es una colección de servicios de cómputo remoto, también llamados servicios web que juntos conforman una plataforma de computación en la nube de Amazon.com desde 2006. Los más conocidos y centrales de estos servicios son Amazon EC2 y Amazon S3. También cuenta con servicios orientados a Big data como Amazon EMR, Amazon Elasticsearch Service y Amazon Athena.


<img  height="100" width="180" src="http://www.aionsolution.com/wp-content/uploads/2017/10/microsoft-azure-640x401.png">

* **Microsoft Azure**: HDInsight de Microsoft Azure es una distribución de Hadoop que funciona en la nube. HDInsight fue diseñado para manejar cualquier cantidad de datos, escalando de terabytes a petabytes bajo demanda. Puede cambiar la cantidad de nodos en cualquier momento y solo se cobra por el cálculo y el almacenamiento que realmente se usa.

<img  height="100" width="300" src="https://cloud.google.com/_static/6d893b1b39/images/cloud/cloud-logo.svg">

* **Cloud Dataflow**: Google Cloud Dataflow es un servicio en la nube totalmente administrado para crear y evaluar pipelines de procesamiento de datos escalables. Los flujos de datos de los pipelines se basan en el modelo de programación Apache Beam y pueden operar tanto en modo por lotes como en streaming.

---

## Distribuidores de Hadoop

<br>

<img  height="100" width="200" src="http://www.fuzzylogix.com/wp-content/uploads/cloudera-logo.png">

* **Cloudera**: Cloudera Inc. es una compañía de software con sede en los Estados Unidos que ofrece software, soporte y servicios basados ​​en Apache Hadoop y capacitación para clientes comerciales. La distribución de Apache Hadoop de código abierto de Cloudera, CDH (Cloudera Distribution incluyendo Apache Hadoop), apunta a implementaciones de clase empresarial de esa tecnología.


<img  height="100" width="180" src="https://hortonworks.com/wp-content/themes/hortonworks/images/svg/ui_logo.svg">

* **Hortonworks**: Hortonworks es una empresa de software de computadoras con sede en Palo Alto, California. La compañía se enfoca en el desarrollo y soporte de Apache Hadoop, un framework que permite el procesamiento distribuido de grandes conjuntos de datos en grupos de computadoras.

<img  height="100" width="200" src="https://mapr.com/assets/images/MapR_logo_red.svg">

* **MapR Technologies**: MapR es una empresa de software empresarial con sede en San José, California, que desarrolla y vende software derivado de Apache Hadoop. La compañía contribuye a 
* proyectos de Apache Hadoop como HBase, Pig, Apache Hive y Apache ZooKeeper.

---

## Seguridad

<br>

<img  height="100" width="300" src="https://www.protegrity.com/wp-content/uploads/2017/02/apache-ranger-logo.png">

* **Apache Ranger**: Ranger es un framework para habilitar, controlar y gestionar la seguridad de datos integral en toda la plataforma Hadoop.


<img  height="100" width="180" src="https://dcassetcdn.com/design_img/343044/36801/36801_2851300_343044_image.png">

* **Sentry**: Apache Sentry es un sistema altamente modular para proporcionar una autorización basada en funciones de granularidad fina a datos y metadatos almacenados en un clúster Apache Hadoop.

<img  height="100" width="200" src="https://jaxenter.de/wp-content/uploads/2014/04/knox.jpg">

* **Knox**: MApache Knox Gateway es una puerta de enlace API REST para interactuar con clústeres de Hadoop. Knox Gateway proporciona un único punto de acceso para todas las interacciones REST con clústeres de Hadoop.

---

Para no entrar en detalle de otras áreas más especificas, a continuación se anexan un par de fuentes donde se pueden detallar los demás componentes que conforman el ecosistema actual de Big Data.

<p align="center">
  <img src="http://mattturck.com/wp-content/uploads/2018/06/Matt-Turck-FirstMark-Big-Data-Landscape-2018.png">
</p>

[Bigdata2018](http://mattturck.com/bigdata2018/ "mattturck 2018")

[Bigdataecosystem](https://bigdataecosystem.knowledgent.com/big-data-ecosystem/#)

 [Pentahoworld](https://www.pentahoworld.com/sites/default/files/2017-11/Understanding-the-Big-Data-Technology-Ecosystem-PWorld2017_0.pdf)


