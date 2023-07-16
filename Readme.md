
::: {#fa103bd1 .cell .markdown}
### PIDA:PROYECTO INDIVIDUAL Nº2
:::

::: {#cdcdcc43 .cell .markdown papermill="{\"duration\":1.6879e-2,\"end_time\":\"2023-06-02T07:44:23.643722\",\"exception\":false,\"start_time\":\"2023-06-02T07:44:23.626843\",\"status\":\"completed\"}" tags="[]"}
```{=html}
<div style="padding: 35px;color:white;margin:10;font-size:200%;text-align:center;display:fill;border-radius:10px;overflow:hidden;background-image: url(https://w0.peakpx.com/wallpaper/957/661/HD-wallpaper-white-marble-white-stone-texture-marble-stone-background-white-stone.jpg)"><b><span style='color:black'>Panorama de la conectividad a Internet en Argentina </span></b> </div>
```
`<br>`{=html}

Este análisis se centra en **visualizar la distribución geográfica** de
varias métricas de acceso a Internet, como cantidad y alcance delos
proveedores del servicio, cantidad de hogares conectados a Internet, las
suscripciones wireless y las suscripciones de banda ancha fija, etc. Las
métricas se estudian a nivel regional en las siguientes provincias con
sus localidades: `Jujuy` (NOA), `Misiones` (NEA) , `Cordoba` (Centro),
`Santiago del Estero` (Centro), `San Juan` (Cuyo), `CABA` (Capital
Nacional), `Neuquen` (Patagonia Norte) y `Santa Cruz` (Patagonia Sur).

El objetivo es crear una serie de **mapas geográficos** en los que las
áreas están sombreadas o modeladas en relación con la variable de datos
que se muestra en el mapa, en este caso, los datos penetración hogareña
de Internet.

Además de arrojar luz sobre el panorama del uso de Internet, este
análisis puede servir como una valiosa herramienta para que los
responsables políticos, los investigadores y las empresas comprendan los
patrones regionales de uso de Internet e impulsen los procesos de toma
de decisiones.

`<br>`{=html}

![](vertopal_0ef5f634eb7a42abb7a68a564690a063/c8d45c53d01754d1c5b8bba85d6bc441ad907a93.jpeg)

`<br>`{=html}

### `<b>`{=html}`<span style='color:#526D82'>`{=html}\|`</span>`{=html} Metadatos y Dominio`</b>`{=html} {#-metadatos-y-dominio}

`<br>`{=html}

1.  **`Provincias y localidades`** Las provincias y localidades son
    divisiones geográficas y político-administrativas de Argentina.

`Provincias:`

Son divisiones territoriales supra-municipales que agrupan varios
municipios o localidades. Cada provincia tiene su propio gobierno, leyes
y autoridades. Suelen tener cierta autonomía respecto al gobierno
central de un país. En Argentina hay 23 provincias y una ciudad autónoma
(CABA).

`Localidades:`

Son divisiones territoriales más pequeñas dentro de una provincia.
Pueden ser ciudades, pueblos, parajes rurales. Cada localidad tiene su
propia administración y gobierno local. Las agrupaciones de localidades
forman los municipios o partidos. Según INDEC en Argentina hay 2.266
localidades urbanas, pero para nuestro análisis conseguimos datos de más
de 4000 localidades, con lo que concluimos que hemos incluido también
localidades no urbanas.

1.  **`Operador de telecomunicaciones`** Un operador de
    telecomunicaciones es una empresa que brinda servicios de telefonía,
    internet y otros servicios de comunicación utilizando
    infraestructura de telecomunicaciones. Sus características son:
    Cuentan con licencias y permisos del Estado para operar redes de
    telecomunicaciones en una región o país. Despliegan la
    infraestructura necesaria como cables de fibra óptica, antenas,
    centrales telefónicas, etc. Proveen servicios minoristas de
    telefonía fija y móvil, internet de banda ancha, televisión paga,
    entre otros. También pueden ofrecer servicios mayoristas a otras
    empresas de telecomunicaciones. Muchos operan redes de alcance
    nacional y tienen millones de clientes, mientras que otras pueden
    ser simples cooperativas locales que ofrecen servicios a poblaciones
    muy reducidas. Están sujetos a regulaciones gubernamentales sobre
    tarifas, competencia, calidad de servicio, etc.

2.  **`Año`**: El análisis se realiza para el año 2022 con el fin de
    reflejar las tendencias más recientes.

3.  **`Velocidad de bajada (conexión)`** - Esta metrica se refiere a la
    rapide, medida en Mbps, a la cual se pueden descargar datos desde
    internet a un dispositivo. Es una métrica importante para medir el
    rendimiento de una conexión de internet. Los valores en las columnas
    de velocidad (Mbps) corresponden a cantidad de hogares con esa
    velocidad de bajada.

`Algunos puntos clave sobre esta métrica:`

Se mide en Megabits por segundo (Mbps). Entre más alta la velocidad, más
rápido es la descarga. Depende de la capacidad tanto del proveedor de
internet como del hardware del usuario. Varía según la tecnología de
conexión (cable, ADSL, fibra óptica, móvil). Fibra óptica ofrece las
velocidades más altas. Influye en experiencia del usuario al descargar
sitios web, video, música, etc. Velocidades bajas causan retrasos. Los
operadores en la actualidad ofrecen rangos desde 50 Mbps a 300 Mbps en
sus planes de internet. Para streaming HD se recomienda mínimo 25 Mbps
de bajada. Gaming requiere al menos 15 Mbps. Tener velocidades de bajada
altas y consistentes es esencial para buena calidad en servicios
digitales.

1.  **`Acceso a la banda ancha`** - Este valor binario refleja la
    presencia o auencia de cada tipo de conexion a Internet en cada
    localidad. Las conexiones fijas de banda ancha, normalmente a través
    de DSL, fibra o cable, suelen ofrecer un servicio más rápido y
    fiable que las conexiones por aire a Internet. Esta métrica es un
    indicador crucial de la infraestructura disponible para servicios
    como el streaming de vídeo de alta calidad, los juegos en línea y
    otras aplicaciones de uso intensivo de datos.

`<br>`{=html}

✔️ **Entendiendo en detalle estos datos, podemos extraer valiosas
perspectivas sobre la conectividad digital global, el acceso a los
servicios digitales, la evolución de la tecnología digital y el
potencial de crecimiento digital en diferentes partes del pais.**
:::

::: {#72b59476 .cell .markdown}
# `<span style="color:#E888BB; font-size: 1%;">`{=html} ANÁLISIS`</span>`{=html} {#-análisis}

```{=html}
<div style="padding: 30px;color:white;margin:10;font-size:170%;text-align:left;display:fill;border-radius:10px;overflow:hidden;background-image: url(https://images.pexels.com/photos/532173/pexels-photo-532173.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1)"><b><span style='color:white'> ANÁLISIS </span></b> </div>
```
En este análisis, nos adentramos en el interesantisimo mundo del
**`<span style='color:#526D82'>`{=html}Acceso a Internet en distintas
latitudes (provincias) del pais, elegidas ademas segun sus ingresos per
capita provincial `</span>`{=html}**. Nos centramos principalmente en
analizar la tecnología disponible, la velocidad de bajada y la cobertura
de distintos proveedores de internet en las distintas Provincias.

Nuestro conjunto de datos, obtenido la pagina del Enacom, contiene una
gran cantidad de información que abarca distintas regiones,
proporcionando una vista de pájaro del acceso Internet en diferentes
partes del pais. Sin embargo, para apreciar realmente la granularidad y
complejidad de estos datos, es imprescindible diseccionarlos en
subconjuntos más específicos.

1.  **Datos regionales**: El primer nivel de nuestro análisis ramifica
    los datos según la columna \"Región\", separando las regiones
    individuales de los datos colectivos. Esta segmentación proporciona
    una comprensión matizada de las diferencias regionales y los
    contrastes de desarrollo, y nos permite centrarnos en el panorama
    digital dentro de estos límites geográficos específicos. Al
    diseccionar los datos de esta manera, podemos desarrollar
    perspectivas específicas para cada región e identificar tendencias y
    patrones únicos.

2.  **Datos del grupo de renta**: La segunda dimensión que exploramos es
    el grupo de renta. Esta categorización segrega a las provincias en
    varias categorias de renta, como provincias de renta baja, renta
    media-baja, renta media-alta y renta alta. Nos hubiera gustado
    realizar un análisis más detallado, examinando los datos según el
    ingreso promedio por localidad y no solo por provincia, ya que este
    último está muy promediado. Sin embargo, lamentablemente no se
    cuenta con información a nivel de localidades que nos permita hacer
    este tipo de segmentación más granular. En la siguiente tabla se
    detallan las provincias que fueron seleccionadas según su renta y su
    distribución geográfica.

      Renta baja   Renta media-baja      Renta media-alta   Renta alta
      ------------ --------------------- ------------------ ------------
      Jujuy        San Juan              Santa Cruz         Córdoba
      Misiones     Santiago Del estero   Neuquén            Caba

    Analizar los datos a través del prisma de los grupos de renta nos
    permite evaluar si existe correlación entre la riqueza de la
    provincia y su acceso y uso de los servicios de Internet. Esta
    segmentación puede revelar notables disparidades en el uso de
    Internet, la accesibilidad y el desarrollo tecnológico en función
    del grupo de renta.

3.  **Datos Poblacionales**: Por último, usamos los datos de la
    población de cada localidad . Esta instantánea nos permite calcular
    la penetración de Internet en función de la población de una
    provincia o localidad, lo que permite ver qué tan extendido está el
    acceso per capita y comparar la población total de una provincias
    con la cantidad de suscripciones a Internet. Las provincias con
    mayor población deberían tener más suscripciones en términos
    absolutos. `<br>`{=html}

```{=html}
<div style="border-radius:10px;border:#526D82 solid;padding: 15px;background-color:#ffffff00;font-size:100%;text-align:left">
   📝A través de este examen multifacético, nuestro análisis promete una comprensión integral y profunda del acceso a internet de calidad a lo largo y ancho del pais, segun la geografía y la segmentacion de ingresos. Esta introducción sirve como hoja de ruta para el viaje que sigue, donde los datos tejen historias de igualdad digital, revelando ideas tan profundas como impactantes.
   </div>
```
`<br>`{=html}
:::

::: {#c3c7ae49 .cell .markdown}
Como se menciono al inicio se usaron los dataset de la pagina de Enacom.
Se realizó una exploracion preliminar para seleccionar los datos
relevantes y poder determinar KPis que permitan llegar a conlusiones e
insigths. El análisis se realizó para el año 2022, último año
disponible, con el fin de reflejar la situación más reciente.

Los datasets se exploraron, analizaron y visualizaron mediante graficas
realizadas con las librerias matplotlib, plotly y seaborn. De este
analisis ([ver EDA](Eda.ipynb)) se obtuvieron 3 Kpis que considero
interesantes:

**KPI 1: Cobertura del Servicio de Internet en el territorio nacional**

Se comenzó con una visión amplia, analizando la penetración nacional de
Internet en los hogares por tipo de conexión. Lo visualizamos con un
gráfico circular, que muestra el porcentaje de hogares con Internet por
tipo de conexión. Luego se profundizo el análisis comparando el acceso
tanto de banda ancha y banda estrecha por provincias de interes,
seleccionadas por su nivel de renta y su distribución geográfica en el
territorio nacional.

**KPI 2: Acceso a internet segun la renta provincial**

Se eligió este Kpi para responder a la pregunta si la renta per cápita
provincial afecta el acceso de sus habitantes a internet de calidad.Es
muy importante conocer si la economía es un impedimento para que la
sociedad de un país acceda a los beneficios que ofrece internet.

**KPI 3: Cantidad y distribución de Operadores de telecomunicaciones por
provincia**:

Como resultado del análisis del acceso a y la calidad de internet de los
habitantes de Argentina decidimos con el último Kpi evaluar la oferta y
cobertura de los distintos operadores.que ofrecen servicios de
telecomunicaciones en el territorio nacional. Conocer la situación
actual de los operadores nos permitirá aconsejar a futuros operadores
que eventualmente quieran ofrecer sus servicios.
:::

::: {#09458212 .cell .markdown}
# `<span style="color:#E888BB; font-size: 1%;">`{=html} CONCLUSIONES`</span>`{=html} {#-conclusiones}

```{=html}
<div style="padding: 30px;color:white;margin:10;font-size:170%;text-align:left;display:fill;border-radius:10px;overflow:hidden;background-image: url(https://images.pexels.com/photos/532173/pexels-photo-532173.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1)"><b><span style='color:white'> CONCLUSIONES </span></b> </div>
```
:::

::: {#1c76c733 .cell .markdown}
Los distintos Kpis analizados nos permiten concluir que la cobertura del
servicio de internet está extendida en la totalidad del territorio
nacional, aunque concentrándose la oferta de distintos operadores en los
centros urbanos más poblados. La realidad socioeconómica de las
provincias no afecta, o lo hace mínimamente, la llegada de tecnologías
más modernas y con mejores velocidades de bajada. La banda estrecha, si
bien todavía permanece distribuida en todo el territorio nacional lo
hace con un porcentaje minoritario dándole paso a tecnologías más
veloces tanto en provincias de renta baja, como en las de rentas alta.
Notablemente en el distrito más poblado y de mejores recursos económicos
las velocidades más bajas tienen todavía mucha prevalencia, lo que
demuestra que la Argentina está en un proceso reciente de transición de
tecnologías antiguas a tecnologías más nuevas que dicho proceso no es
acelerado por una mayor renta per cápita o mayor población..
:::

::: {#1b08e5df .cell .markdown}
## **Fuentes**

```{=html}
</div>
```
-   [Documentacion Pandas](https://pandas.pydata.org/docs/)
-   [Documentacion Matplotlib](https://matplotlib.org/stable/index.html)
-   [Documentacion Plotly](https://plotly.com/python/)
-   [Enacom](https://datosabiertos.enacom.gob.ar/home) `<br>`{=html}
:::

::: {#3eecd40a .cell .markdown}
## **Contacto**
:::
