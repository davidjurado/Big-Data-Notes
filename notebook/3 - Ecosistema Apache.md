# El ecosistema Big Data en el ambiente Apache

Se mencionaron algunos miembros del ecosistema de Big Data en el anterior [documento](https://github.com/davidjurado/Big-Data-Notes/blob/master/notebook/1.md) . Sin embargo, el ecosistema de Apache es demasiado grande y necesita ser definido por separado, a continuación se mencionan los componentes que conforman el ecosistema Big Data en el ambiente Apache (y algunos otros que no son de apache pero se complementan).

---

### Sistemas de archivos distribuidos

|Herramienta|Observaciones|
| --------- |  :------------|
Apache HDFS |El Sistema de archivos distribuidos de Hadoop (HDFS) ofrece una forma de almacenar archivos de gran tamaño en varias máquinas. Hadoop y HDFS se obtuvieron a partir del documento de Google File System (GFS).
Red Hat GlusterFS|GlusterFS es un sistema de archivos de almacenamiento conectado a la red de escalamiento horizontal. GlusterFS fue desarrollado originalmente por Gluster, Inc., luego por Red Hat, Inc., después de su compra de Gluster en 2011.
Quantcast File System QFS|QFS es un paquete de software de sistema de archivos distribuido de código abierto para MapReduce a gran escala u otras cargas de trabajo de procesamiento por lotes. Fue diseñado como una alternativa al HDFS de Apache Hadoop, destinado a ofrecer un mejor rendimiento y rentabilidad para los clusters de procesamiento a gran escala.
Ceph Filesystem|Ceph es una plataforma de almacenamiento de software libre diseñada para presentar el almacenamiento de objetos, bloques y archivos desde un solo clúster de computadora distribuida. Los principales objetivos de Ceph son distribuirse por completo sin un solo punto de falla, escalable al nivel exabyte y libremente disponible.
Lustre file system|El sistema de archivos Lustre es un sistema de archivos distribuido de alto rendimiento destinado a entornos de red  más grandes y de alta disponibilidad. Tradicionalmente, Lustre está configurado para administrar dispositivos de disco de almacenamiento de datos remotos dentro de una Red de área de almacenamiento (SAN), que es dos o más dispositivos de disco conectados de forma remota que se comunican mediante un protocolo de interfaz de sistema de computadora pequeña (SCSI).
Alluxio|Alluxio, el primer sistema de almacenamiento distribuido virtual centrado en la memoria del mundo, unifica el acceso a los datos y une los frameworks de cálculo y los sistemas de almacenamiento subyacentes. Las aplicaciones solo necesitan conectarse con Alluxio para acceder a los datos almacenados en cualquier sistema de almacenamiento subyacente.
GridGain|GridGain es un proyecto de código abierto con licencia bajo Apache 2.0. Una de las piezas principales de esta plataforma es el Acelerador In-Memory Apache Hadoop, cuyo objetivo es acelerar HDFS y Map / Reduce incorporando datos y cálculos en la memoria.
XtreemFS|XtreemFS es un sistema de almacenamiento de propósito general y cubre la mayoría de las necesidades de almacenamiento en una sola implementación. Es de código abierto, no requiere hardware especial ni módulos de kernel, y puede montarse en Linux, Windows y OS X. XtreemFS se ejecuta distribuido y ofrece resistencia a través de la replicación.

---

### frameworks de programación distribuida

|Herramienta|Observaciones|
| --------- |  :------------|
Apache Hadoop| Es un framework de código abierto de Apache escrito en java que permite el procesamiento distribuido de grandes conjuntos de datos en grupos de computadores utilizando modelos de programación simples.
Apache Map reduce | Es un modelo de programación que permite distribuir el trabajo en diversos nodos del cluster
Apache YARN |(Yet another resource negociator) Es un framework para la programación de trabajos y la administración de recursos del clúster.
Apache Flink|Apache Flink presenta poderosas abstracciones de programación en Java y Scala, un tiempo de ejecución de alto rendimiento y optimización automática de programas.
Apache Spark |Spark es un motor rápido de procesamiento de datos en memoria con APIs de desarrollo elegantes y expresivas para permitir a los trabajadores de datos ejecutar de manera eficiente la transmisión, el aprendizaje automático o las cargas de trabajo SQL que requieren un acceso iterativo rápido a los conjuntos de datos.
Apache TEZ| Tez es una propuesta para desarrollar una aplicación genérica que se puede usar para procesar DAG de tareas complejas de procesamiento de datos y se ejecuta de forma nativa en Apache Hadoop YARN. Tez generaliza el paradigma MapReduce a un framework más poderoso basado en expresar cálculos como un gráfico de flujo de datos.
Apache Ignite|Es una plataforma en memoria distribuida para computación y transacciones en conjuntos de datos a gran escala en tiempo real. Incluye una almacenamiento en memoria de clave-valor distribuida, capacidades de ejecución SQL, map-reduce, estructuras de datos distribuidos, consultas continuas, subsistemas de mensajería y eventos, integración de Hadoop y Spark. Ignite está construido en Java y proporciona una API para .NET y C ++.
Apache Pig|Pig proporciona un motor para ejecutar flujos de datos en paralelo en Hadoop. Incluye un lenguaje, Pig Latin, para expresar estos flujos de datos. Pig Latin incluye operadores para muchas de las operaciones de datos tradicionales (join, sort, filter, etc.), así como la capacidad de los usuarios para desarrollar sus propias funciones de lectura, procesamiento y escritura de datos. Pig corre en Hadoop.
Apache Storm|Storm es un procesador de eventos complejos (CEP) y un framework de cálculo distribuido escrito predominantemente en el lenguaje de programación Clojure. Es un sistema de computación distribuido en tiempo real para el procesamiento rápido de grandes flujos de datos.
Apache Flink|Apache Flink (anteriormente llamado Stratosphere) presenta poderosas abstracciones de programación en Java y Scala, un tiempo de ejecución de alto rendimiento y optimización automática de programas, es un sistema de procesamiento de datos y una alternativa al componente MapReduce de Hadoop. Viene con su propio tiempo de ejecución, en lugar de ejecutarse sobre MapReduce.
Apache Apex|Apache Apex es una plataforma empresarial basada en Yarn que unifica el procesamiento streaming y el procesamiento por lotes. Procesa grandes datos en streaming de una forma altamente escalable, de alto rendimiento, tolerante a fallas, segura, distribuida y de fácil operación.
---

### Herramientas de inserción de datos en HDFS

La mayoría de los datos se originan fuera del clúster de Hadoop. Estas herramientas permiten insertar datos en HDFS.

|Herramienta|Observaciones|
| --------- |  :------------|
Flume |Flume es un servicio distribuido, confiable y disponible para recopilar, agregar y mover grandes cantidades de datos de registro de manera eficiente. Tiene una arquitectura simple y flexible basada en flujos de datos de transmisión. Es robusto y tolerante a fallas con mecanismos de confiabilidad ajustables y muchos mecanismos de conmutación por error y recuperación. Utiliza un modelo de datos extensible simple que permite la aplicación analítica en línea.
Chukwa |Agregador de registro a gran escala y análisis.
Sqoop |Sistema para la transferencia masiva de datos entre HDFS y áreas de almacenamiento de datos estructuradas como RDBMS.
Kafka |Sistema distribuido de suscripción y publicación para procesar grandes cantidades de datos de transmisión. Kafka es una Message Queue desarrollada por LinkedIn que persiste mensajes en el disco de una manera muy eficiente. Debido a que los mensajes se conservan, tiene la interesante capacidad de rebobinar una transmisión y volver a consumir los mensajes.

---

### Consulta de datos en HDFS

|Herramienta|Observaciones|
| --------- |  :------------|
Java MapReduce |Mapreduce nativo en Java
Hadoop Streaming |Mapreduce en otros lenguajes (Ruby, Python)
Pig |Pig proporciona un motor para ejecutar flujos de datos en paralelo en Hadoop. Incluye un lenguaje, Pig Latin, para expresar estos flujos de datos. Pig Latin incluye operadores para muchas de las operaciones de datos tradicionales (join, sort, filter, etc.), así como la capacidad de los usuarios para desarrollar sus propias funciones de lectura, procesamiento y escritura de datos. Pig corre en Hadoop. Utiliza tanto el sistema de archivos distribuidos de Hadoop, HDFS, como el sistema de procesamiento de Hadoop, MapReduce.
Hive |Hive proporciona una capa SQL sobre HDFS. Los datos se pueden consultar utilizando SQL en lugar de escribir código Java Map Reduce.
Stinger / Tez |Próxima generación de Hive.
Cloudera Search |Búsqueda de texto en HDFS
Impala |Proporciona consultas en tiempo real sobre Big Data. Desarrollado por Cloudera.
Presto |Desarrollado por Facebook, es un motor SQL que en promedio es 10 veces más rápido que Hive para ejecutar consultas en grandes conjuntos de datos almacenados en Hadoop y en otros lugares.

---

### SQL en Hadoop / HBase

|Herramienta|Observaciones|
| --------- |  :------------|
Hive |Hive proporciona una capa SQL sobre HDFS. Los datos se pueden consultar utilizando SQL en lugar de escribir código Java Map Reduce.
Stinger / Tez |Próxima generación de Hive.
Impala |Proporciona consultas en tiempo real sobre Big Data. Desarrollado por Cloudera.
Presto |Desarrollado por Facebook, es un motor SQL que en promedio es 10 veces más rápido que Hive para ejecutar consultas en grandes conjuntos de datos almacenados en Hadoop y en otros lugares.
Phoenix |Apache Phoenix es un capa SQL sobre HBase entregado como un controlador JDBC integrado al cliente y dirigido a consultas de baja latencia sobre datos HBase. Apache Phoenix toma la consulta SQL, la compila en una serie de escaneos HBase y orquesta la ejecución de esos escaneos para producir conjuntos de resultados JDBC regulares.
Apache Drill|Es la versión de código abierto del sistema Dremel de Google, que está disponible como un servicio de infraestructura llamado Google BigQuery. En los últimos años, han surgido sistemas de fuente abierta para abordar la necesidad de procesamiento por lotes escalable (Apache Hadoop) y procesamiento de flujo (Storm, Apache S4).
Apache Zeppelin|Es un Notebook basado en la web de múltiples propósitos que brinda funciones de ingestión de datos, exploración de datos, visualización, uso compartido y colaboración en Hadoop y Spark.

---

## Procesamiento en Streaming

|Herramienta|Observaciones|
| --------- |  :------------|
Storm |Es un framework de cálculo distribuido escrito predominantemente en el lenguaje de programación Clojure. Es un sistema de computación distribuido en tiempo real para el procesamiento rápido de grandes flujos de datos. Storm es una arquitectura basada en el paradigma master-workers.
Apache S4 | S4 (Simple Scalable Streaming System) es una plataforma de uso general, distribuible, escalable, parcialmente tolerante a fallas y conectable que permite a los programadores desarrollar fácilmente aplicaciones para procesar flujos continuos e ilimitados de datos.
Samza |Apache Samza es un frework de procesamiento de flujo distribuido. Utiliza Apache Kafka para mensajería y Apache Hadoop YARN para proporcionar tolerancia a fallas, aislamiento de procesador, seguridad y administración de recursos.
Malhar |Plataforma Hadoop nativa, escalable, tolerante a los fallos y con estado completo.

---

### Almacenamiento NoSQL

|Herramienta|Observaciones|
| --------- |  :------------|
HBase |Base de datos distribuida no relacional. Operaciones de lectura y escritura en tiempo real en tablas muy grandes orientadas a columnas (BDDB: Big Data Data Base). Es el sistema de respaldo para salidas de trabajos de MapReduce. Es la base de datos Hadoop.
Cassandra |Base de datos NoSQL distribuida, es un BDDB. MapReduce puede recuperar datos de Cassandra. Puede ejecutarse sin HDFS o encima de HDFS. HBase y sus sistemas de soporte requeridos se derivan de lo que se conoce de los diseños originales de Google BigTable y Google File System.
Redis |Redis es una almacenaiento de estructuras de datos de código abierto, en red, con durabilidad opcional. Está escrito en ANSI C. En su capa externa, el modelo de datos de Redis es un diccionario que mapea las claves de los valores. Una de las principales diferencias entre Redis y otros sistemas de almacenamiento estructurados es que Redis admite no solo cadenas, sino también tipos de datos abstractos.
Amazon SimpleDB |Amazon SimpleDB es una base de datos NoSQL de alta disponibilidad que descarga el trabajo de administración de bases de datos. Los desarrolladores simplemente almacenan y consultan elementos de datos a través de solicitudes de servicios web y Amazon SimpleDB hace el resto.
Voldermort |Voldemort es un almacén de datos distribuidos que está diseñado como un almacén de clave-valor utilizado por LinkedIn para el almacenamiento de alta escalabilidad.
Accumulo |Almacenamiento distribuido de claves / valores es un sistema robusto, escalable y de almacenamiento y recuperación de datos de alto rendimiento. Apache Accumulo se basa en el diseño BigTable de Google y está construido sobre Apache Hadoop, Zookeeper y Thrift. Accumulo es un software creado por la NSA con características de seguridad.
Kudu|sistema de almacenamiento de datos en formato columnar que permite realizar consultas analíticas sobre estos de forma más fácil y con un gran rendimiento. 

### Hadoop en la nube

|Herramienta|Observaciones|
| --------- |  :------------|
Amazon Elastic Map Reduce (EMR) |Es un servicio web que facilita procesar grandes cantidades de datos de manera eficiente. Amazon EMR utiliza el proceso de Hadoop combinado con varios productos de AWS para realizar tareas como la indexación web, la extracción de datos, el análisis de archivos de registro, el aprendizaje automático, la simulación científica y el almacenamiento de datos.
Microsoft Azure|Para la analítica, Azure tiene Data Lake Analytics, que utiliza U-SQL propietario con SQL y C++, así como HDInsight, un servicio basado en Hadoop. 
Hadoop on Google Cloud |El servicio de datos BigQuery de Google utiliza una interfaz similar a SQL que es intuitivo para que la mayoría de los usuarios –incluso los no técnicos– lo aprendan.
Whirr |Herramienta para activar y administrar fácilmente los clústeres Hadoop en servicios en la nube como Amazon / RackSpace.

### Herramientas de flujo de trabajo

|Herramienta|Observaciones|
| --------- |  :------------|
Oozie |Sistema de planificador de trabajos de flujo para trabajos de MapReduce utilizando DAG (gráficos acíclicos directos). El coordinador de Oozie puede activar trabajos por tiempo y disponibilidad de datos
Azkaban|Gestión del flujo de trabajo de Hadoop. Es un planificador de trabajos por lotes creado por Linkedin.
Cascading |Framework para que los desarrolladores de Java creen sólidas aplicaciones de Data Analytics y Data Management en Apache Hadoop.
Scalding |Biblioteca de Scala que facilita la especificación de trabajos de Hadoop MapReduce.
Lipstick |Permite obtener una visualización del flujo de trabajo Pig

### frameworks de serialización

|Herramienta|Observaciones|
| --------- |  :------------|
Avro |Apache Avro es un framework para modelar, serializar y realizar llamadas de procedimiento remoto (RPC). Los datos Avro se describen mediante un esquema, y ​​una característica interesante es que el esquema se almacena en el mismo archivo que los datos que describe, por lo que los archivos son autodescriptivos.
Trevni |Formato de archivo de columna
Protobuf |Biblioteca de serialización popular (no es un proyecto de Hadoop).
Parquet |Formato de almacenamiento en columna disponible para cualquier proyecto en el ecosistema de Hadoop, independientemente de la elección del framework de procesamiento de datos, el modelo de datos o el lenguaje de programación.

### Sistemas de monitoreo

|Herramienta|Observaciones|
| --------- |  :------------|
Hue |Aplicación web para interactuar con Apache Hadoop. No es una herramienta de desarrollo, es una interfaz web de código abierto que admite Apache Hadoop y su ecosistema.
Ganglia |Sistema de monitoreo general del host. Hadoop puede publicar métricas en Ganglia.
Open TSDB |Colector de métricas y visualizador.
Nagios |Monitoreo de la infraestructura de TI.

### Aplicaciones y plataformas

|Herramienta|Observaciones|
| --------- |  :------------|
Mahout |Librería de Machine learning y procesamiento matematico que corre sobre Hadoop.
Giraph |Apache Giraph es un sistema iterativo de procesamiento de gráficos creado para una gran escalabilidad. Por ejemplo, actualmente se usa en Facebook para analizar el gráfico social formado por los usuarios y sus conexiones.
Lily |Lily unifica Apache HBase, Hadoop y Solr en una plataforma de datos interactiva e integrada

### Coordinación Distribuida

|Herramienta|Observaciones|
| --------- |  :------------|
Zookeeper |ZooKeeper es un servicio centralizado para mantener la información de configuración, nombrar y proporcionar sincronización distribuida.
Book keeper |Servicio de registro distribuido basado en ZooKeeper.

### Data Analytics en Hadoop

|Herramienta|Observaciones|
| --------- |  :------------|
R language |Entorno de software para computación y gráficos estadísticos.
RHIPE |Integra R y Hadoop.

### Procesamiento de mensajes distribuidos

|Herramienta|Observaciones|
| --------- |  :------------|
Kafka |Sistema distribuido de suscripción y publicación.
Akka |Sistema de mensajería distribuida con actores.
RabbitMQ |Sistema de mensajería MQ distribuido.

### Herramientas de Business Intelligence (BI)

|Herramienta|Observaciones|
| --------- |  :------------|
Datameer |La compañía se centra en el análisis y la visualización de big data. 
Tableau |Empresa de software que desarrolla productos de visualización de datos interactivos que se enfocan en inteligencia empresarial.
Pentaho |Ofrece un conjunto de programas para generar inteligencia empresarial.
SiSense |Su producto de inteligencia de negocios incluye un dispositivo de respaldo con tecnología integrada en el chip que permite a los usuarios no técnicos unirse y analizar grandes conjuntos de datos de múltiples fuentes
SumoLogic |Permite crear, ejecutar y proteger aplicaciones AWS, Azure, Google Cloud Platform o híbridas, da un servicio analítico de datos de máquina nativo de la nube para administración de registros y mediciones de series de tiempo.

---

### frameworks basados ​​en YARN

|Herramienta|Observaciones|
| --------- |  :------------|
Samza |Apache Samza es un framework de procesamiento de flujo distribuido. Utiliza Apache Kafka para mensajería y Apache Hadoop YARN para proporcionar tolerancia a fallas, aislamiento de procesador, seguridad y administración de recursos.
Spark |Spark es un motor rápido de procesamiento de datos en memoria con APIs de desarrollo elegantes y expresivas para permitir a los trabajadores de datos ejecutar de manera eficiente la transmisión, el aprendizaje automático o las cargas de trabajo SQL que requieren un acceso iterativo rápido a los conjuntos de datos.
Malhar |Plataforma Hadoop nativa, escalable, tolerante a los fallos y con estado completo, desarrollada por DataTorrent
Storm |Procesamiento de flujo rápido desarrollado por Twitter.
Hoya (HBase en YARN) | La herramienta Hoya es una herramienta Java y actualmente está dirigida por CLI.

### Librerias / frameworks

|Herramienta|Observaciones|
| --------- |  :------------|
Kiji |Crear aplicaciones Big Data en tiempo real en Apache HBase
Elephant Bird |Códigos de compresión y serializadores para Hadoop.
Summing Bird |MapReduce en Storm
Apache Crunch |Líneas simples y eficientes de MapReduce para Hadoop y Spark
Apache DataFu |Trabaja con datos a gran escala en Hadoop. El proyecto se inspiró en la necesidad de bibliotecas estables y bien probadas para la extracción de datos y las estadísticas.
Continuuity |Crea aplicaciones en HBase fácilmente

### Gestión de datos

|Herramienta|Observaciones|
| --------- |  :------------|
Apache Falcon |Gestión de datos, linaje de datos

### Seguridad

|Herramienta|Observaciones|
| --------- |  :------------|
Apache Sentry |Es un sistema altamente modular para proporcionar una autorización basada en funciones de granularidad fina a datos y metadatos almacenados en un clúster Apache Hadoop.
Apache Knox |Es una puerta de enlace API REST para interactuar con clústeres de Hadoop. Knox Gateway proporciona un único punto de acceso para todas las interacciones REST con clústeres de Hadoop.

###  frameworks de prueba

|Herramienta|Observaciones|
| --------- |  :------------|
MrUnit |framework de pruebas unitarias para Java MapReduce
PigUnit |Para testear scripts de Pig

### Adicional

|Herramienta|Observaciones|
| --------- |  :------------|
Shark (Hive on Spark) | Apache shark es un motor de consulta distribuido desarrollado por la comunidad de código abierto. Este motor de consulta se usa principalmente para datos de Hadoop. Proporciona un rendimiento mejorado y resultados analíticos de alta calidad para los usuarios de Hive.
