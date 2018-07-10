# Bases de datos en HDFS

### Apache HBase

Apache HBase es una base de datos NoSQL de código abierto que proporciona acceso de lectura/escritura en tiempo real a esos grandes conjuntos de datos.

HBase escala linealmente para manejar grandes conjuntos de datos con miles de millones de filas y millones de columnas, y combina fácilmente fuentes de datos que usan una amplia variedad de estructuras y esquemas diferentes. HBase se integra de forma nativa con Hadoop y funciona sin problemas junto con otros motores de acceso a datos a través de YARN.

### Apache Cassandra

Apache Cassandra, un proyecto Apache de alto nivel nacido en Facebook y creado en Dynamo de Amazon y BigTable de Google, es una base de datos distribuida para administrar grandes cantidades de datos estructurados en muchos servidores básicos, al tiempo que proporciona un servicio altamente disponible y ningún punto de falla. Apache Cassandra ofrece capacidades que las bases de datos relacionales y otras bases de datos NoSQL simplemente no pueden igualar: disponibilidad continua, rendimiento de escala lineal, simplicidad operativa y fácil distribución de datos en múltiples centros de datos y zonas de disponibilidad en la nube.

### Apache Accumulo

Accumulo es un sistema de almacenamiento y recuperación de datos latencia con seguridad de nivel de celda. Pueden almacenar y administrar grandes conjuntos de datos en un clúster. Accumulo usa el HDFS de Apache Hadoop para almacenar sus datos y Apache ZooKeeper para el consenso. Mientras muchos usuarios interactúan directamente con Accumulo, varios proyectos de código abierto usan Accumulo como su tienda subyacente.

### Apache CouchBD

Apache CouchDB es un software de base de datos de código abierto que se enfoca en la facilidad de uso y una arquitectura escalable. Tiene una arquitectura de base de datos NoSQL orientada a documentos y se implementa en el lenguaje orientado a la concurrencia Erlang; usa JSON para almacenar datos, JavaScript como su lenguaje de consulta usando MapReduce y HTTP para una API.

### Apache kudu

Apache Kudu es un almacén de datos orientado a columnas de fuente abierta y gratuita del ecosistema Apache Hadoop. Es compatible con la mayoría de los marcos de procesamiento de datos en el entorno de Hadoop. Proporciona una capa de almacenamiento completa de Hadoop para permitir análisis rápidos en datos rápidos.

### MongoDB

Sistema de base de datos orientado a documentos. Es parte de la familia de sistemas de bases de datos NoSQL. En lugar de almacenar datos en tablas como se hace en una base de datos relacional "clásica", MongoDB almacena datos estructurados como documentos similares a JSON.

### arangodb

ArangoDB es un sistema de base de datos multi-modelo nativo desarrollado por triAGENS GmbH. El sistema de base de datos admite tres modelos de datos importantes (clave / valor, documentos, gráficos) con un núcleo de base de datos y un lenguaje de consulta unificado AQL (Lenguaje de consulta ArangoDB). El lenguaje de consulta es declarativo y permite la combinación de diferentes patrones de acceso a datos en una sola consulta. ArangoDB es un sistema de base de datos NoSQL, pero AQL es similar en muchos sentidos a SQL.

---

### GeoMesa

GeoMesa es un conjunto de herramientas de código abierto que permite realizar consultas y análisis geoespaciales a gran escala en sistemas informáticos distribuidos. GeoMesa proporciona indexación espacio-temporal en la parte superior de las bases de datos Accumulo, HBase, Google Bigtable y Cassandra para el almacenamiento masivo de datos de puntos, líneas y polígonos. GeoMesa también proporciona un procesamiento de flujo casi en tiempo real de datos espacio-temporales mediante la estratificación de la semántica espacial en la parte superior de Apache Kafka. A través de GeoServe GeoMesa facilita la integración con una amplia gama de clientes de mapeo existentes sobre las API y protocolos estándar OGC (Open Geospatial Consortium) como WFS y WMS. GeoMesa es compatible con 
Apache Spark para el análisis geoespacial distribuido personalizado.

### ESRI GIS Tools para Hadoop

Para muchos grandes conjuntos de datos, la ubicación es un componente crucial para comprender verdaderamente los patrones y tendencias subyacentes. Sin ubicación, los conjuntos de datos son menos valiosos, o en circunstancias extremas, sin sentido. GIS Tools para Hadoop funciona con grandes datos espaciales (Big Data con ubicación) y le permite completar el análisis espacial utilizando la potencia del procesamiento distribuido en Hadoop.

### AsterixDB

AsterixDB es un BDMS (Big Data Management System) con un amplio conjunto de funciones que lo distingue de otras plataformas Big Data. Su conjunto de características lo hace adecuado para las necesidades modernas, como el almacenamiento de datos web y el almacenamiento y análisis de datos sociales. AsterixDB tiene Modelo de datos, Escalabilidad, Almacenamiento nativo, Almacenamiento externo e Indexación.

### HadoopGIS

Es un sistema de almacenamiento de datos espaciales escalable y de alto rendimiento para ejecutar consultas espaciales a gran escala en Hadoop. Hadoop-GIS admite múltiples tipos de consultas espaciales en MapReduce a través de particiones espaciales, motor de consulta espacial personalizable RESQUE, ejecución de consultas espaciales paralelas implícitas en MapReduce y métodos efectivos para enmendar resultados de consultas mediante el manejo de objetos límite.
