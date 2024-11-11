# Proyecto1-DashboardExcel 📊 

- **Descripción del Proyecto** 📝​

El proyecto se basa en un analisis descriptivo de una empresa multinacional que vende al por mayor articulos de camping y actividades recreativas y deportes al aire libre.

En lineas generales a la empresa, en el periodo de estudio, le va muy bien, con un margen promedio de ganancia por encima del 40%. 

A medida que avanzaba el análisis exploratorio, se identificó que, según el criterio del analista, sería altamente beneficioso para la empresa considerar una expansión en el mercado de artículos de golf. Esto se debe a la creciente demanda en este sector, su alto potencial de rentabilidad y, especialmente, a la baja participación actual de la empresa en países con una fuerte cultura golfista, lo que presenta una oportunidad de crecimiento significativa.

- **Estructura del Proyecto** 🗂️

        ├── VentasProductos_RawData/                    # Datos crudos
        ├── VentasProductos_KPI_Dashboard/              # Aqui se encuentran los KPI y Dashboard
        ├── VentasProductos_EDAs_Corr_Covz/             # Analsis Exploratorios, correlacion y covarianza
        ├── README.md                                   # Descripción del proyecto

- **Instalación y Requisitos** 🛠️

El proyecto está desarrollado íntegramente en Microsoft Excel, por lo que solo se necesita tener acceso a esta herramienta. La versión recomendada es Excel 2016 o superior, para aprovechar las características avanzadas de gráficos y tablas dinámicas.

- **Limpieza de datos**🧹

-    Se identificaron y eliminaron dos filas duplicadas para evitar redundancias en los datos.

-    Para el tratamiento de valores nulos o faltantes en las columnas de revenue y cantidad, se siguió el siguiente proceso:

*Revenue:* Para completar los datos faltantes de revenue, primero se identificó el precio unitario de venta de cada producto en el conjunto de datos de órdenes. Luego, en una nueva hoja llamada "Calculo_medias_nulos", se copió el precio unitario de todos los productos con valores faltantes de revenue.

En esta hoja, se utilizó la función =MEDIANA(D2:D591) para calcular la mediana de los precios unitarios, lo que permitió obtener un valor representativo para cada producto.

Con las medianas calculadas, se empleó una fórmula de búsqueda en la hoja principal (tabla1) para rellenar los valores de revenue faltantes mediante la función =BUSCARV([@Product];'Calculo_medias_nulos'!$A$2:$B$17;2;0). Así, se trajo el precio unitario calculado en la hoja de apoyo para cada producto.

*Cantidad:* Para los valores faltantes en la columna cantidad, se utilizó una regla de tres basada en otra fila que contenía el mismo producto y Gross margin similar. Esto permitió estimar los valores faltantes de manera coherente y consistente, respetando la proporcionalidad entre productos similares.

- **Resultados y Conclusiones** 🕵️‍♂️

La empresa ha logrado un sólido desempeño financiero, con ingresos de 3.775 millones de euros y un margen de ganancia del 41,32% en el periodo de estudio. La compañia se enfoca en el sector de productos para actividades al aire libre, incluyendo principalmente accesorios personales, equipos de camping y artículos de golf, siendo el canal web nuestro principal medio de venta (85% de las ventas totales).

A nivel internacional, contamos con presencia en 21 países, destacándose Estados Unidos como nuestro mercado líder, representando el 17,25% de nuestras ventas, seguido de Japón. En el segmento de golf, los mejores resultados se han obtenido en Estados Unidos, Canadá y Japón, países con un alto número de campos de golf. No obstante, se han identificado oportunidades de crecimiento en paises como el Reino Unido, Australia y Suecia, donde la popularidad del golf y la infraestructura existente presentan un alto potencial de desarrollo de ventas.

La demanda de productos de golf muestra estacionalidad, concentrándose en el primer y segundo trimestre del año, lo que coincide con el inicio de la temporada en el hemisferio norte. Esto permite a los golfistas prepararse para aprovechar el clima cálido, impulsando nuestras ventas de equipos de golf en los meses de primavera y verano.

- **Recomendaciones a hacer para expandir el negocio de golf** 📈

La empresa debería expandir su presencia en mercados clave como Reino Unido, Australia y Suecia. Sabemos que estos países tienen una fuerte cultura golfista, por lo que se enfocarán las campañas de marketing en ellos, trabajando de la mano con tiendas deportivas locales y patrocinando eventos y torneos para fortalecer nuestra marca.

En las tiendas de golf y deportes donde está presente la empresa, se aumentará la variedad de productos más demandados, como Woods e Irons, e introducirá modelos exclusivos y personalizados para satisfacer las necesidades de los golfistas más exigentes. Además, se implementarán promociones cruzadas para incentivar la compra de accesorios junto con los equipos principales, lo que ayudará a aumentar las ventas de categorías menos populares.

Se aprovecharán los primeros trimestres del año (Q1 y Q2), cuando el interés por el golf es más alto, para aumentar el inventario de los productos más demandados y lanzar campañas de marketing pretemporada. En los meses más fríos, durante Q3 y Q4, se ofrecerán packs de invierno con descuentos en productos básicos y accesorios, ideales para prácticas en interiores o como regalos para las fiestas.

La estrategia está diseñada para captar la atención de golfistas en cada momento clave, asegurando que la marca esté presente cuando más la necesitan, y ofreciendo productos y promociones que resuenen con sus pasiones y hábitos de compra.

- **Próximos Pasos** 🔄 

        - Mejorar en la limpieza de datos, documentar a medida que se fueron haciendo cambios a la base original.
        - Mejorar en el diseño de dashboards.


- **Contribuciones** 🤝 

Las contribuciones son bienvenidas para mejorar este proyecto. Si deseas colaborar, abre un pull request o crea una issue para discutir tus ideas. Se valoran especialmente las contribuciones en las áreas de análisis de datos y visualización.

- **Autores y Agradecimientos** ✒️ 

**Agustin Salomon**

Repositorios Github
https://github.com/aSalomon96

mi LinkedIn https://www.linkedin.com/in/agustin-salomon/

Agradecimientos especiales a mis profesoras Ana y Jeancha por su apoyo y orientación durante el desarrollo de este proyecto.