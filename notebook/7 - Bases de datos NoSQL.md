# Bases de datos NoSQL

NoSQL (originalmente se refiere a "no SQL" o "no relacional", posteriormente extendido a no sólo SQL) es un término genérico para una clase definida de base de datos que proporcionan un mecanismo para el almacenamiento y la recuperación de datos que se modelan de formas diferentes de las relaciones tabulares usadas en las bases de datos relacionales. Las bases de datos NoSQL se utilizan cada vez más en Big Data y las aplicaciones web en tiempo real. Los sistemas NoSQL, a veces, también se llaman "No sólo SQL" ("No sólo SQL") para enfatizar que pueden soportar lenguajes de consulta similares a SQL.


<img src="https://i.imgur.com/LondgHi.png">

Las motivaciones para este enfoque incluyen: simplicidad de diseño, escalado "horizontal" más simple y un control más preciso de la disponibilidad. Las estructuras de datos utilizadas por las bases de datos NoSQL son diferentes de las utilizadas por defecto en las bases de datos relacionales, lo que hace que algunas operaciones sean más rápidas en NoSQL. La idoneidad particular de una base de datos NoSQL dada depende del problema que debe resolver. En ocasiones, las estructuras de datos utilizadas por las bases de datos NoSQL también se consideran "más flexibles" que las tablas de bases de datos relacionales.

<img src="https://i.imgur.com/Hh1MpD5.png">

### índices espaciales

Los índices espaciales son utilizados por bases de datos espaciales (bases de datos que almacenan información relacionada con objetos en el espacio) para optimizar las consultas espaciales. Los tipos de índice convencionales no manejan de manera eficiente las consultas espaciales, como la diferencia entre dos puntos o si los puntos caen dentro de un área espacial de interés.

Algunas soluciones NoSQL incluyen soporte para datos geoespaciales de forma nativa o con una extensión. Otros no están diseñados para aplicaciones geoespaciales, pero se han implementado para admitir datos geoespaciales. 

|Nombre|Estrategia de indexación|Tipo de datos|Tipos de Queries|
|----|----|----|----|
|DynamoDB|geohash|point|BBOX,radius
|GeoCouch|R-tree|point/line/poly|BBOX,radius
|Cloudant|R*-tree|GeoJSON|BBOX,radius,arbitrary shape
|Lucene/Solr|geohash|point|BBOX,radius
|Orchestrate.io|geohash|point|BBOX,radius
|Azure Cosmos DB (DocumentDB)|-|-|-
|MongoDB|geohash/quadtree|GeoJSON|BBOX,radius,arbitrary shape
|Neo4j|-|-|-|
|CouchDB with GeoCouch extension|-|-|-|
|Cassandra|-|-|-|
|Redis|-|-|-|
|HBase|-|-|-|
|Oracle NoSQL|-|-|-|
|Amazon DynamoDB|-|-|-|
|Couchbase|-|-|-|
|Memcached|-|-|-|
|PostGIS|-|-|-|
|BigTable|-|-|-|
