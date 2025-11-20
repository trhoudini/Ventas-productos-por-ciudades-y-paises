README.MD

Título del Proyecto

📊 Análisis de ventas de productos en el mundo entre el 2011 y el 2014.


📖 Descripción del Proyecto

El objetivo de este proyecto final es demostrar la capacidad de demostrar los conocimientos que he adquirido a lo largo de todo el programa de Data & Analytics de thePower. En el mismo, me he centrado en realizar un EDA y un dashboard de un conjunto de datos resultado de la unión de dos bases de datos.

Para este trabajo he combinado dos datasets procedentes de Kaggle:

•	Superstore Sales Dataset (SuperStoreOrders.csv): https://www.kaggle.com/datasets/laibaanwer/superstore-sales-dataset

•	World Cities Dataset (world-cities.csv): https://www.kaggle.com/datasets/juanmah/world-cities/data

Tras unirlos, se generó un dataset final de más de 50.000 filas y 20 columnas, que permite analizar el comportamiento comercial de un amplio catálogo de productos vendidos en distintos países y regiones del mundo.

Columnas del dataset:

● order_id: Identificador único del pedido realizado.

● order_date: Fecha en la que se realizó el pedido.

● ship_date: Fecha en la que el pedido fue enviado al cliente.

● ship_mode: Tipo de envío utilizado (por ejemplo: entrega estándar, rápida o el mismo día).

● customer_name: Nombre del cliente que realizó la compra.

● segment: Segmento de mercado al que pertenece el cliente (por ejemplo: consumidor, empresa, hogar).

● state: Estado o provincia donde se realizó el pedido.

● country: País donde se encuentra el cliente o se registró la venta.

● market: Región comercial global (por ejemplo: Asia Pacífico, Europa, América Latina, etc.).

● region: Subdivisión geográfica dentro del mercado (por ejemplo: norte, sur, centro).

● product_id: Identificador único del producto vendido.

● category: Categoría general del producto (por ejemplo: Tecnología, Muebles, Suministros de oficina).

● sub_category: Subcategoría del producto (por ejemplo: Sillas, Teléfonos, Papel).

● product_name: Nombre o descripción del producto.

● sales: Valor total de las ventas de ese pedido (importe monetario).

● quantity: Cantidad de unidades del producto vendidas.

● discount: Descuento aplicado al producto en esa venta (en proporción, entre 0 y 1).

● profit: Beneficio neto obtenido por la venta del producto (ventas menos costes).

● shipping_cost: Coste del envío asociado al pedido.

● order_priority: Nivel de prioridad asignado al pedido (por ejemplo: alta, media, baja).

● year: Año en que se realizó el pedido.

● admin_name: Nombre administrativo de la división territorial (estado o provincia).

● latitud: Coordenada geográfica de latitud correspondiente al lugar del pedido.

● longitud: Coordenada geográfica de longitud correspondiente al lugar del pedido.

● poblacion: Población estimada de la ciudad o región donde se realizó el pedido.

● latitud_pais: Coordenada geográfica de latitud correspondiente del país desde donde se hace el pedido.

● longitud_pais: Coordenada geográfica de longitud correspondiente del país desde donde se hace el pedido.

● poblacion_pais: Población estimada del país desde donde se hace el pedido.

El análisis se ha centrado en comprender la estructura general del negocio, su evolución temporal, los segmentos de clientes que más compran, los modos de envío y niveles de prioridad de los pedidos, las categorías de productos más vendidas, subcategorías más vendidas, los factores económicos a tener en cuenta, el comportamiento geográfico de las ventas y la rentabilidad del negocio.

Para analizar todo el proyecto he tenido que realizar todas estas fases:

1. Unión de las bases de datos.

2. Análisis preliminar de la BD unida.

3. Limpieza de la BD.

4. Análisis descriptivo de la BD.

5. Análisis estadístico de la BD.

6. EDA (Análisis exploratorio de los datos).

7. Dashboard con los datos más importantes.


📁 Estructura del Proyecto

ventas-productos-por-paises/

├── data/                                                                    # Carpeta de datos

│  ├── output/                                                           # Datos procesados / limpios

│   │   └── basededatos_limpia.csv                          # Base de datos limpia

│  ├── raw/                                                                 # Datos originales sin procesar

│   │   ├── basededatos_unida.csv                          # Unión de las 2 bases de datos

│   │   ├── SuperStoreOrders.csv                             # Primera base de datos

│   │    └── world-cities.csv                                         # Segunda base de datos

├── notebook/                                                           # Notebooks Jupyter con el análisis

│   ├── 01-Union_bases_de_datos.ipynb              # Unión de las bases de datos

│   ├── 02-Analisis_preliminar.ipynb                      # Análisis preliminar de los datos

│   ├── 03-Limpieza_basededatos_unida.ipynb   # Limpieza de datos

│   ├── 04-Analisis_descriptivo.ipynb                     # Análisis descriptivo de los datos

│   ├── 05- Analisis_estadistico.ipynb                     # Análisis estadístico de los datos

│   ├── 06-EDA.ipynb                                                 # Análisis EDA (Análisis exploratorio)

│   ├── 07-Dashboard.docx                                       # Gráfico con KPIS más relevantes

│    └──- 08-Informe_explicativo_analisis.docx       # Informe explicativo del análisis 

├── src/                                                                        # Código fuente de apoyo

│  ├── _pycache_/                                                 # Caché          

│   └── soporte.py                                                        # Funciones reutilizables o utilidades

├── .gitignore                                                           # Archivos y carpetas ignorados por Git

└── README.md                                                          # Descripción completa del proyecto


🛠️ Instalación y Requisitos

- Análisis y EDA

Esta parte se ha realizado en Python desde Visual Studio Code (VSCode). Requiere las siguientes bibliotecas:

•	Pandas

•	Matplotlib

•	Seaborn

- Dashboard

Se ha generado a través de Google Sheets.


📊 Resultados y Conclusiones

•	Estructura general del negocio:

Las ventas se distribuyen principalmente en los mercados de APAC, US y EU, concentrando la mayor parte de los ingresos en US. El mercado LATAM muestra una menor participación, aunque con potencial de crecimiento.

•	Evolución temporal:

Las ventas presentan una tendencia positiva a lo largo de los años, alcanzando su punto máximo en 2014, lo que refleja un crecimiento sostenido del negocio y una consolidación de las operaciones internacionales.

•	Segmentos de clientes:  

El segmento Consumer es el más relevante en volumen de ventas, seguido por Corporate, mientras que Home Office representa la menor proporción. Esto sugiere una mayor dependencia del consumidor final en la estructura comercial.

•	Modos de envío y prioridades:  

El modo de envío Standard Class es el más utilizado, lo que indica una preferencia por opciones más económicas y de mayor volumen. En cuanto a las prioridades de pedido, la mayoría son de tipo Medium y High, reflejando un equilibrio entre urgencia y planificación.

•	Categorías de producto:

Las categorías Office Supplies genera la mayor cantidad de operaciones, mientras que Technology y Furniture presenta un menor volumen pero con mayores márgenes de beneficio por transacción.

•	Subcategorías de producto:

Las subcategorías Phones, Storage, Chairs, Bookcases y Copiers concentran el mayor volumen de ventas del catálogo, mientras que Fasteners, Labels y Envelopes registran un nivel de ventas significativamente menor, aunque pueden aportar mayores márgenes relativos por transacción al operar en nichos más específicos.

•	Factores económicos:

Existe una relación positiva entre el coste de envío y las ventas, aunque débil, mientras que el descuento presenta un impacto negativo sobre los beneficios, lo que confirma la sensibilidad del margen a las políticas de precio.

•	Comportamiento geográfico:

Las ventas se concentran en países del hemisferio norte y en ciudades con poblaciones medias, lo que sugiere una red comercial establecida en zonas urbanas desarrolladas. Los valores extremos de latitud y longitud se asocian con menor actividad comercial.

•	Rentabilidad:

La mayoría de las transacciones se sitúan en beneficios bajos o negativos, lo que pone de manifiesto la necesidad de revisar estrategias de descuento, costes logísticos y márgenes de producto.

Conclusiones finales:

•	Se ve un incremento constante de las ventas de 2011 a 2014.

•	Dependiente del segmento Consumer.

•	Concentrado en mercados consolidados (US, APAC, EU).

•	Rentable en determinadas categorías, pero con presión de margen debida a los descuentos.


🔄 Próximos Pasos

•	Añadir modelos predictivos para estimar ventas en años futuros.

•	Uso de datos históricos de años anteriores para completar el análisis.

•	Implementar clustering para segmentar clientes o productos.

•	Desarrollar un dashboard interactivo en Power BI o Looker Studio.

•	Integrar datos externos como inflación, PIB o índices logísticos.


🤝 Contribuciones

Si te interesa mejorar o extender este proyecto, las contribuciones son bienvenidas.


✒️ Autores y Agradecimientos

Autor: Francisco Troyano Martínez.  

Contacto: troyano1406@gmail.com .

GitHub: https://github.com/trhoudini .

