# ¿Qué es Big Data?

Se han creado diferentes definiciones de Big Data, una de las más antiguas y que aún es considerada como la definición de referencia es la de [Gartner(2001)](https://www.gartner.com/it-glossary/big-data):

***"Big Data son activos de información de gran volumen, alta velocidad y gran variedad, que demandan formas rentables e innovadoras de procesamiento, lo que permiten un mejor conocimiento, toma de decisiones y automatización de procesos".***

Dicho de otro modo, Big Data está formado por conjuntos de datos de mayor tamaño y más complejos, especialmente procedentes de nuevas fuentes de datos. Estos conjuntos de datos son tan voluminosos que el software de procesamiento de datos convencional sencillamente no puede gestionarlos. Sin embargo, estos volúmenes masivos de datos pueden utilizarse para abordar problemas que antes no hubiera sido posible solucionar. Big Data no son solo datos, sino que se ha convertido en un tema completo, que involucra diversas herramientas, técnicas y frameworks.

---

## Las V's de Big Data

<p align="center">
  <img width="460" height="300" src="https://1.bp.blogspot.com/-4PXnx5bSWO8/WH2-DfIpFZI/AAAAAAAAAg4/efnThIh6esMYtjYxwoktHFNmRrDiX5MqQCLcB/s640/7Vs_of_Big_Data.PNG">
</p>

Con la definición dada por Gartner se definieron 3 características claves de Big Data, las cuales se denominaron las 3 V's de Big Data.

* **Volumen**: Esta es la característica principal que define a Big Data como "Big". Todos los días se procesan grandes volúmenes de datos los cuales puede poseer un valor desconocido, como publicaciones de usuarios en una red social, registros de clics en una página web o aplicación para móviles o dispositivos con diferentes sensores.  Con el crecimiento de los datos que se están generando y que se deben almacenar, encontramos que el almacenamiento en Gigabytes en realidad no es suficiente. Debido a esta razón, en el mundo de hoy se analizan desde decenas de Terabytes hasta en cientos de petabytes, Exabytes, Zettabytes y Yottabytes.

* **Velocidad**: Se refiere a qué tan rápido se acceden y procesan los datos. Tradicionalmente se programaba que los datos fueran analizados y actualizados cada cierto periodo de tiempo, hoy en día, las tendencia se basa en el análisis de datos en tiempo real, por lo que las operaciones de datos en intervalos grandes no son en absoluto útiles.

* **Variedad**: La variedad hace referencia a los diversos tipos de datos disponibles. Los tipos de datos convencionales eran estructurados y podían organizarse fácilmente en una base de datos relacional. La tendencia se dirige al análisis de datos que se presentan en como datos no estructurados. Los tipos de datos no estructurados y semiestructurados, como el texto, audio o vídeo, requieren de un pre procesamiento adicional para poder obtener significado.

A medida que pasaron los años se determinó que los anteriores 3 aspectos no son suficientes para describir Big Data en su totalidad, es por esto que en los últimos años se han identificado otras características (que también comienzan con la letra V). Partiendo de las originales [3 V's](https://blogs.gartner.com/doug-laney/files/2012/01/ad949-3D-Data-Management-Controlling-Data-Volume-Velocity-and-Variety.pdf) se ha llegado a hablar de [4 V's](http://www.ibmbigdatahub.com/infographic/four-vs-big-data), [5 V's](https://www.wired.com/insights/2013/05/the-missing-vs-in-big-data-viability-and-value/), [6 V's](https://insidebigdata.com/2013/09/12/beyond-volume-variety-velocity-issue-big-data-veracity/), [7 V's](https://datafloq.com/read/3vs-sufficient-describe-big-data/166), [10 V's](https://mapr.com/blog/top-10-big-data-challenges-serious-look-10-big-data-vs/) e incluso se han llegado a describir [42 V's](https://www.elderresearch.com/blog/42-v-of-big-data), a continuación se describen algunas de las V's adicionales mayormente aceptadas:

* **Veracidad**: Tener una gran cantidad de datos de gran volumen entrando a alta velocidad no tiene valor si esos datos son incorrectos. Los datos incorrectos pueden causar muchos problemas tanto para las organizaciones como para los consumidores. Por lo tanto, las organizaciones deben garantizar que los datos sean correctos y que los análisis realizados sobre los datos sean confiables. Especialmente en la toma de decisiones automatizada, donde ya no interviene ningún ser humano, debe asegurarse de que tanto los datos como los análisis sean acertados.

* **Variabilidad**: La variabilidad se centra principalmente en comprender e interpretar correctamente los significados de los datos brutos que dependen del contexto. Esto se requiere principalmente cuando se trabaja en procesamiento del lenguaje natural. Por ejemplo, Hay algunas palabras que pueden tener múltiples significados y el significado exacto depende del contexto en que se utiliza, es importante que el significado exacto se interprete correctamente para realizar un análisis adecuado.

* **Visualización**: se refiere a cómo se presentan los datos para la toma de decisiones, es hacer que toda esa gran cantidad de datos comprensibles de una manera que sea fácil de entender y leer. Con los análisis y visualizaciones correctos, los datos brutos pueden utilizarse, de lo contrario, los datos en bruto permanecen esencialmente inútiles. Las visualizaciones, por supuesto, no significan gráficos ordinarios o gráficos circulares. Significan gráficos complejos que pueden incluir muchas variables de datos mientras siguen siendo comprensibles y legibles.

* **Valor**: Los datos poseen un valor intrínseco. Sin embargo, no tienen ninguna utilidad hasta que dicho valor se descubre. Hoy en día, gran parte del valor que ofrecen las grandes compañías tecnológicas procede de sus datos, que analizan constantemente para generar una mayor eficiencia y desarrollar nuevos productos. Identificar el valor de los datos se trata de todo un proceso de descubrimiento que requiere que los analistas, usuarios empresariales y ejecutivos se planteen las preguntas correctas, identifiquen patrones, tomen decisiones informadas y predigan comportamientos.

---

## La historia de Big Data

Si bien el concepto "Big Data" en sí mismo es relativamente nuevo, los orígenes de los grandes conjuntos de datos se remontan a las décadas de 1960 y 1970, donde se sitúan los origines de este universo con los primeros centros de datos y el desarrollo de las bases de datos relacionales.

Alrededor de 2005, la gente empezó a darse cuenta de la cantidad de datos que generaban los usuarios a través de Facebook, YouTube y otros servicios online. Ese mismo año, se desarrollaría Hadoop, un framework de código abierto creado específicamente para almacenar y analizar grandes conjuntos de datos. En esta época, también empezaría a adquirir popularidad NoSQL.

El desarrollo de Framewoks de código abierto tales como Hadoop y más recientemente Spark, sería esencial para el crecimiento de Big Data, pues estos hicieron que Big Data resultase más fácil de usar y más barato de almacenar. En los años siguientes, el volumen de Big Data se ha disparado. Los usuarios continúan generando enormes cantidades de datos, pero ahora los humanos no son los únicos que lo hacen.

Con la llegada del Internet de las cosas (IoT), hay un mayor número de objetos y dispositivos conectados a Internet que generan datos sobre patrones de uso de los clientes y rendimiento de los productos.

Aunque Big Data ha llegado lejos, su utilidad no ha hecho más que empezar. El Cloud Computing ha ampliado aún más las posibilidades de Big Data. La nube ofrece una escalabilidad realmente elástica, donde los desarrolladores pueden simplemente crear clústeres remotos y ajustarlos a sus necesidades.

---

## Ciclo de vida de Big Data

1. **Evaluación de caso comercial**

    El comienzo del ciclo de vida de Big Data comienza con una evaluación sólida del caso comercial. Antes de que se pueda iniciar cualquier proyecto de Big Data, debe quedar claro cuáles deberían ser los objetivos comerciales y los resultados del análisis de datos. Se debe comenzar con el fin en mente y definir claramente los objetivos y los resultados deseados del proyecto. Se podrían realizar muchas formas diferentes de análisis de datos, pero ¿cuál es exactamente la razón para invertir tiempo y esfuerzo en el análisis de datos? Al igual que con cualquier buen caso comercial, la propuesta debe estar respaldada por datos financieros.

2. **Identificación de datos**

    La etapa de identificación de datos determina el origen de los datos. Antes de analizar los datos, es importante saber cuáles serán las fuentes de los datos. Especialmente si los datos se adquieren de proveedores externos, es necesario identificar claramente cuál es la fuente original de los datos y qué tan confiable (veracidad) es el conjunto de datos. La segunda etapa del ciclo de vida de Big Data es muy importante, porque si los datos de entrada no son confiables, los datos de salida tampoco serán confiables.

3. **Adquisición de datos y filtrado**

    La Fase de Adquisición y Filtrado de Datos se basa en la etapa anterior del ciclo de vida de Big Data. En esta etapa, los datos se recopilan de diferentes fuentes, tanto dentro de la empresa como fuera de ella. Después de la adquisición, se realiza un primer paso de filtrado para filtrar los datos corruptos. Además, los datos que no son necesarios para el análisis serán filtrados también.

4. **Extracción de datos**

    Algunos de los datos identificados en las dos etapas anteriores pueden ser incompatibles con la herramienta Big Data que realizará el análisis real. Para tratar este problema, la etapa de extracción de datos está dedicada a extraer diferentes formatos de datos de conjuntos de datos y transformarlos en un formato que la herramienta Big Data puede procesar y analizar. La complejidad de la transformación y el grado en que es necesario transformar los datos depende en gran medida de la herramienta de Big Data que se ha seleccionado.

5. **Validación y purificación de datos**

    Los datos que no son válidos generan resultados no válidos. Para garantizar que solo se analicen los datos apropiados, se requiere la etapa de Validación y limpieza de datos. Durante esta etapa, los datos se validan contra un conjunto de condiciones y reglas predeterminadas para garantizar que los datos no estén corruptos. Un ejemplo de una regla de validación sería excluir a todas las personas mayores de 100 años, ya que es muy poco probable que los datos sobre estas personas sean correctos debido a limitaciones físicas.

6. **Agregación y representación de datos**

    Los datos pueden distribuirse en múltiples conjuntos de datos, lo que requiere que el conjunto de datos se una para realizar el análisis real. Para garantizar que solo se analicen los datos correctos en la siguiente etapa, puede ser necesario integrar múltiples conjuntos de datos. La etapa de Agregación y Representación de Datos está dedicada a integrar conjuntos de datos múltiples para llegar a una vista unificada. Además, la agregación de datos acelerará en gran medida el proceso de análisis de la herramienta Big Data, ya que no se requerirá que la herramienta junte diferentes tablas de diferentes conjuntos de datos, acelerando enormemente el proceso.

7. **Análisis de datos**

    La etapa Análisis de datos está dedicada a llevar a cabo la tarea de análisis real. Ejecuta el código o algoritmo que realiza los cálculos que conducirán al resultado real. El análisis de datos puede ser simple o realmente complejo, según el tipo de análisis requerido. En esta etapa, se generará el "valor real" del proyecto Big Data. Si todas las etapas anteriores se han ejecutado cuidadosamente, los resultados serán objetivos y correctos.

8. **Visualización de datos**

    La capacidad de analizar cantidades masivas de datos y encontrar información útil es una cosa, comunicar los resultados de una manera que todos puedan entender es algo completamente diferente. La etapa de visualización de datos está dedicada al uso de técnicas y herramientas de visualización de datos para comunicar gráficamente los resultados del análisis para una interpretación efectiva por parte de los usuarios. Con frecuencia, esto requiere trazar puntos de datos en cuadros, gráficos o mapas de calor.

9.  **Utilización de los resultados del análisis**

    Después de que se haya realizado el análisis de datos y se haya presentado el resultado, el paso final del ciclo de vida de Big Data es utilizar los resultados en la práctica. Los resultados del análisis están dedicados a determinar cómo y dónde pueden utilizarse los datos procesados para aprovechar el resultado del proyecto Big Data.

---

## Algunas ventajas de Big Data y de la analítica de datos

* Mejora de la toma de decisiones: Con Big Data se pueden analizar datos pasados para hacer predicciones sobre el futuro. Por lo tanto, las empresas no solo pueden tomar mejores decisiones para su día a día, sino también prepararse para el futuro. Esto les da una ventaja competitiva y proporciona un marco más ágil para la toma de decisiones y el manejo de riesgos.

* Reducción de costes: Big Data proporciona la inteligencia empresarial necesaria para reducir costes y mejorar la eficiencia de las operaciones. El análisis de Big Data puede proporcionar información sobre el impacto de diferentes variables en el proceso de producción, ayudando así a las industrias a tomar mejores decisiones.

* Nuevos productos y servicios: Analizando los datos pasados sobre lanzamientos de productos y cruzando esos datos con datos de opiniones de clientes es posible mejorar los nuevos productos que se pretenden lanzar en el futuro. Además de esto, el análisis de mercado en tiempo real permite a las empresas comprender los cambios en la demanda y en el comportamiento de los consumidores lo que ayuda a una comercialización orientada al cliente. Una mayor demanda de servicios personalizados también puede potenciarse mediante el análisis de las necesidades del consumidor, las preferencias y los comportamientos de compra.

* Feedback en tiempo real: Incluso en los momentos en los que es necesario tomar una decisión inmediata, Big Data es un arma muy poderosa puesto que permite recibir y procesar los datos a tiempo real y contar con la información necesaria rápidamente. Big Data es por encima de todo una tecnología ágil y veloz que permite por ejemplo obtener información a tiempo real del lanzamiento de un producto o el resultado de una estrategia.

* Conocimiento del mercado: El conocimiento del mercado en el que se opera puede ayudar no solo a la toma de decisiones, sino también a la localización de posibles oportunidades mediante el tratamiento de estos datos. También puede ayudar a predecir posibles escenarios e incluso a conocer mejor a a los consumidores, mediante un análisis segmentado.

---

## Casos de uso de Big Data

Big Data puede ayudar a abordar una serie de actividades empresariales, a continuación se muestran algunas de ellas:

#### Desarrollo de productos
Empresas como Netflix y P&G usan Big Data para prever la demanda de los clientes. Construyen modelos predictivos para nuevos productos y servicios clasificando atributos clave de productos anteriores y actuales y modelando la relación entre dichos atributos y el éxito comercial de las ofertas. Además, P&G utiliza los datos y la analítica de grupos de interés, redes sociales, mercados de prueba y avances de salida en tiendas para planificar, producir y lanzar nuevos productos.

#### Mantenimiento predictivo
Los factores capaces de predecir fallos mecánicos pueden estar profundamente ocultos entre datos estructurados (año del equipo, marca o modelo de una máquina) o entre datos no estructurados que cubren millones de entradas de registros, datos de sensores, mensajes de error y temperaturas de motor. Al analizar estos indicadores de problemas potenciales antes de que estos se produzcan, las organizaciones pueden implantar el mantenimiento de una forma más rentable y optimizar el tiempo de servicio de componentes y equipos.

#### Experiencia del cliente
Disponer de una vista clara de la experiencia del cliente es más posible que nunca. Big Data permite recopilar datos de redes sociales, visitas a páginas web, registros de llamadas y otras fuentes de datos para mejorar la experiencia de interacción, así como maximizar el valor ofrecido. Se formulan ofertas personalizadas, reducen las tasas de abandono de los clientes y gestionan las incidencias de manera proactiva.

#### Fraude y conformidad
Big Data ayuda a identificar patrones en los datos que pueden ser indicativos de fraude, al tiempo que concentra grandes volúmenes de información para agilizar la generación de informes normativos.

#### Aprendizaje automático (Machine Learning)
El aprendizaje automático es actualmente un tema de gran popularidad. Los datos (concretamente Big Data) son uno de los motivos de que así sea. Ahora, en lugar de programarse, las máquinas pueden aprender. Esto es posible gracias a la disponibilidad de Big Data para crear modelos de aprendizaje automático.

#### Eficiencia operativa
Big Data permite analizar y evaluar la producción, la opinión de los clientes, las devoluciones y otros factores para reducir las situaciones de falta de stock y anticipar la demanda futura. Big Data también puede utilizarse para mejorar la toma de decisiones en función de la demanda de mercado en cada momento.

#### Impulso de la innovación
Big Data puede ayudar a innovar mediante el estudio de las interdependencias entre seres humanos, instituciones, entidades y procesos, y, posteriormente, mediante la determinación de nuevas formas de usar dicha información. Utilizar las perspectivas que ofrecen los datos puede mejorar las decisiones financieras y consideraciones de planificación. 

---

## Desafíos de Big Data

Si bien es cierto que Big Data promete mucho, también se enfrenta a desafíos.

En primer lugar, Big Data se caracteriza por su gran tamaño. Aunque se han desarrollado nuevas tecnologías para el almacenamiento de datos, el volumen de datos duplica su tamaño cada dos años aproximadamente. Las organizaciones continúan esforzándose por mantener el ritmo de crecimiento de sus datos y por encontrar formas de almacenarlos eficazmente.

Pero no basta con almacenar los datos. Para ser de algún valor, los datos deben poder utilizarse, y esto depende de su conservación. Disponer de datos limpios (es decir, datos relevantes que permitan un análisis significativo) requiere una gran cantidad de trabajo. Los científicos de datos dedican entre un 50 y un 80 por ciento de su tiempo a seleccionar y preparar los datos antes de que estos puedan utilizarse.

Por último, la tecnología de Big Data cambia a un ritmo rápido. Hace unos años, Apache Hadoop era la tecnología más conocida y utilizada para gestionar operaciones de Big Data. Más tarde, en 2014, entraría en juego Apache Spark. Hoy en día, el enfoque óptimo parece ser una combinación de ambos frameworks. Mantenerse al día en cuanto a tecnología de Big Data supone un desafío constante.