# Bases de datos NoSQL

Los índices espaciales son utilizados por bases de datos espaciales (bases de datos que almacenan información relacionada con objetos en el espacio) para optimizar las consultas espaciales. Los tipos de índice convencionales no manejan de manera eficiente las consultas espaciales, como la diferencia entre dos puntos o si los puntos caen dentro de un área espacial de interés.

Algunas soluciones NoSQL incluyen soporte para datos geoespaciales de forma nativa o con una extensión. Otros no están diseñados para aplicaciones geoespaciales, pero se han implementado para admitir datos geoespaciales. Algunas bases de datos NoSQL que se usan actualmente para administrar datos geoespaciales incluyen: MongoDB (código abierto), BigTable (desarrollado por Google, propietario, utilizado en Google Earth), Cassandra (desarrollado por Facebook, ahora de código abierto y mantenido por Apache), CouchDB (código abierto Apache), entre otras.

|name|Estrategia de indexación|Tipo de datos|Tipos de Queries|
|----|----|----|----|
|DynamoDB|geohash|point|BBOX,radius
|GeoCouch|R-tree|point/line/poly|BBOX,radius
|Cloudant|R*-tree|GeoJSON|BBOX,radius,arbitrary shape
|Lucene/Solr|geohash|point|BBOX,radius
|Orchestrate.io|geohash|point|BBOX,radius
|DocumentDB|-|-|-
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
|Azure Cosmos DB|-|-|-|
