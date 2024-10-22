---
title: "XII CVE - Creando modelos de distribución de especies para usos en conservación con Wallace, la nueva aplicación Shiny basada en R"
output: html_document
---
### Horario
Viernes 14 de febrero de 10:30 a.m. - 12:30 p.m.

### Webinar 
El webinar se realizará por medio de la plataforma *Zoom*, por lo que recomendamos se asegure de tener buena conexión de internet y descargar el software [aquí](https://zoom.us/download). 

Una vez descargue Zoom en su computadora puede unirse al webinar siguiente [este link](https://zoom.us/j/623908394?pwd=blFnRVpEMDZuVllSQS9YaVNWM2l3QT09). 


### Organizadores: 
Erica Johnson (City College of New York, CUNY)
Gonzalo Pinilla-Buitrago (City College of New York, CUNY)

### Descripción del webinar: 

Los modelos de distribución de especies constituyen una valiosa herramienta para la biología de la conservación, ya que nos permiten estimar los límites de su distribución geográfica actual, así como realizar proyecciones sobre su distribución potencial en otras áreas geográficas o períodos temporales. A pesar de los numerosos avances metodológicos en la construcción y evaluación de este tipo de modelos, el acceso a métodos de vanguardia generalmente se encuentra restringidos a aquellos investigadores con conocimiento de lenguajes de programación, resultando en una barrera para la comunidad científica y otros usuarios. Wallace es una nueva aplicación Shiny para la elaboración de modelos de distribución de especies, basada en el lenguaje de programación R.

Wallace cuenta con una interfaz gráfica que facilita la implementación de técnicas avanzadas para el modelado de distribución de especies. Igualmente, Wallace provee materiales educativos para guiar a usuarios (i.e. viñeta, texto “in-situ”, videos); tanto nuevos como expertos, en las prácticas de modelado, junto a referencias bibliográficas relevantes. Cada sesión de modelado puede ser exportada como un archivo R script documentado con el fin de asegurar su reproducibilidad y facilitar la documentación de resultados. En este taller, presentaremos los fundamentos del modelado de distribuciones utilizando Wallace y demostraremos las características del software, así como sus posibles aplicaciones para la biología de la conservación.

### Cuestionarios pre- y post-webinar
Por favor ayúdanos a mejorar nuestro curso respondiendo los siguientes cuestionarios:

-	[Cuestionario pre-taller](https://forms.gle/MejQDUqctrK47AGY9)
-	[Cuestionario post-taller](https://forms.gle/7v8WAuCXZxepJ5ue7)

### Introducción a modelos de distribución de especies
[Diapositivas](WallaceCVE_feb2020.pdf)

### Datos 
[Datos de presencia GBIF de *Ara ararauna* y variables bioclimáticas WorldClim](https://github.com/johnsonojeda/WallaceCVE/raw/master/data.zip)

### Introducción a Wallace
Wallace es una plataforma para modelar nichos y distribuciones de especies modular y reproducible escrita en R. Esta aplicación guía a los usuarios en el proceso analítico desde la adquisición de datos hasta la visualización de las predicciones del modelo por medio de mapas interactivos, integrando esta serie de operaciones complejas en una interfaz gráfica sencilla. 

#### 1.	Antes de utilizar Wallace 
Asegúrate de que hayas instalado la versión mas reciente tanto de:

-	R (instrucciones para [descarga en Windows y Mac](https://cran.r-project.org/)) 

-	RStudio (instrucciones para [descarga para Windows y Mac](https://rstudio.com/products/rstudio/download/); escoja la versión gratuita).

#### 2.	Instalando Wallace
Puedes instalar Wallace vía CRAN y correr esta aplicación utilizando el siguiente código de R: 
```r
install.packages("wallace") #instalación del paquete Wallace en R

library(wallace) #cargar el paquete al espacio de trabajo en R

run_wallace() #correr la aplicación Shiny
```

Versiones en desarrollo (“development versions”) puden ser descargadas desde Github utilizando el siguiente código de R (no recomendado para usuarios nuevos): 
```r
install.packages("devtools") #instalación del paquete devtools en R

devtools::install_github("wallaceEcoMod/wallace") #instalación del paquete Wallace en R

library(wallace) #cargar el paquete al espacio de trabajo en R

run_wallace() #correr la aplicación Shiny
```

#### 3. Recursos de Wallace
-	[Página web](https://wallaceecomod.github.io/) (inglés)
-	[¿Cómo utilizar Wallace? Viñeta](https://wallaceecomod.github.io/vignettes/wallace_vignette.html) (inglés)
-	[Grupo Google](https://groups.google.com/forum/#!forum/wallaceecomod)

###¿Deseas contribuir con Wallace? 
El equipo de Wallace está en búsqueda de colaboradores externos. Si tienes una idea que crees puede ser integrado como un módulo del software por favor contáctanos al siguiente email *wallaceEcoMod@gmail.com*. 

Cabe destacar que se le dará prioridad a aquellas personas que hayan desarrollado un paquete de R listo para la integración a Wallace.