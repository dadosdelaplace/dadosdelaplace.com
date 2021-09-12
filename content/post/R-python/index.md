---
authors:
- admin
categories: []
date: "2021-09-12T00:00:00Z"
draft: false
featured: false
image:
  caption: 'https://www.yosoyungamer.cloud/anuncian-el-regreso-de-fight-club-con-fight-club-3/'
  focal_point: ""
  preview_only: false
lastmod: "2021-09-12"
projects: []
subtitle: '¿Qué lenguaje elegir para el análisis de datos?'
summary: "¿Qué lenguaje elegir para el análisis de datos?"
tags:
- Programación en R
- conceptos básicos R
title: "¿Qué lenguaje elegir? R, Python o Matlab: la batalla final"
---

> **Quiero empezar con el análisis de datos: ¿qué lenguaje debo elegir?**

Esta es una de las preguntas más habituales que recibimos muchos/as de los/as que nos dedicamos al análisis de datos y la divulgación estadística en redes: **de todo el vasto universo de lenguajes de programación, ¿cuál elegir?**

Y te voy a decepcionar con la respuesta: **depende**.

![](rajoy.)

El propósito de esta entrada no es hacer una disertación sobre el mundo de la programación (tienes una [breve cronología](#cronologia) al final de la entrada) sino **servir de guía a un usuario muggle para elegir** entre los tres lenguajes más comunes en la ciencia (sin requerir grandes conocimientos de informática): ¿`R`, `Python` o `Matlab`?

* ¿Necesito una **ejecución rápida** (tareas diarias iguales, por ejemplo)? 

* ¿Estoy dispuesto a sacrificar tiempo en ejecución a cambio de una **curva de aprendizaje más rápida** y un **tiempo en la programación** más corto?

Aunque los tres lenguajes son diferentes entre sí, he optado por ellos ya que comparten una virtud: son **lenguajes de alto nivel**. Como regla general, los **lenguajes de alto nivel** suelen ser más lentos en ejecución pero mucho **más cómodos y sencillos** para un usuario medio, mientras que **lenguajes de bajo nivel** (`C` o `FORTRAN`) son mucho más rápidos en ejecución, pero **requieren de un mayor conocimiento** informático. Y aunque algunos científicos con conocimientos en programación siguen optando por los lenguajes de bajo nivel, la **mayoría de la comunidad científica** optan en sus análisis por lenguajes que puedan aprender rápido, al no requerir en general de una gran eficiencia en tiempos de ejecución (sacrificando algunos segundos o minutos en la ejecución, a cambio de poder ser más o menos autosuficientes en su programación).

&nbsp;

# Consejo: descarta Matlab, apuesta por el software libre

Debido a su potencia, seguramente si eres un **usuario medio** que necesita cosas sencillas para el análisis de datos, **las tres herramientas** te puedan cubrir la mayoría de tus necesidades. Sin embargo, hay un aspecto que diferencia `Matlab` (`M`) de los otros dos lenguajes: **`Matlab` es de pago**. Como sucede con lenguajes/herramientas como `SPSS` (IBM) o `SAS`, `Matlab`  requiere de una **licencia de pago**. Esta desventaja a priori puede que no nos parezca relevante a la hora de decidirnos por un lenguaje de programación, ya que probablemente lo hayas podido usar de forma «gratuita», bien porque hayas encontrado una forma de **piratearlo** (en el caso de `Matlab`, bastante sencillo), bien porque tengas acceso a una licencia académica o corporativa, siendo tu universidad o empresa la que tenga un **acuerdo de licencias**.

**¿Es entonces una desventaja real?** Sí, pero no por el precio que tengas que pagar por su uso, sino por lo que ello implica: su **código no es de libre uso**. `Matlab`, como todos los programas de software de pago, son de código cerrado, lo que **impide acceder al totalidad del código** de las funciones internas del lenguaje, lo cual a su vez **impide la colaboración entre usuarios**: `Matlab` **no permite la instalación directa de código validado por la comunidad** de usuarios (puedes copiar y pegar código que encuentres en la red, pero sin tener una garantía de que realiza lo que promete, ni de compatibilidad, ni de integración, ni de documentación).

Otra aspecto diferencial para descartar `Matlab` es que, como probablemente hayas experimentado si has trabajado con dicha herramienta, tiene un alto consumo de recursos. No solo **consume una monstruosa cantidad de espacio en el disco duro** tras sus instalación (mientras que instalar `R` puede ocupar 100MB, una instalación de `Matlab` puede superar los 5GB), sino que además **consume una gran cantidad de memoria RAM** en su ejecución: es una herramienta tan potente pero tan rígida en su configuración que «por si lo necesitases» implementa toda una compleja infraestructura.

Y es que precisamente una de las desventajas (en mi opinión) de `Matlab`, aunque pueda parecer contradictorio, es su propósito general, ya que **pretende abarcar tantos campos** que, salvo necesidades muy especiales donde no hay competidor (modelización y simulación de ecuaciones diferenciales y cálculo matricial, entre ellas, no es casualidad que se llame 
**MAT**rix **LAB**oratory), seguramente **puedas encontrar otro lenguaje o software libre cuyas funcionalidades sean más acordes** y específicas a tu necesidad, como puede ser el caso de `R` o `Python` respecto al análisis de datos. 

&nbsp;

# ¿`R` o `Python`?

Se acabó el *hype*, vamos a pinchar la burbuja: **ambos son igualmente válidos para el análisis de datos**.

En mi caso particular, durante la carrera aprendí lenguajes como `C++`, `FORTRAN`, `PASCAL` o `Java`, mi TFM lo realicé en `Python` y mi tesis doctoral la hice entera en `Matlab` (limitaciones ajenas), por lo que no fue hasta finalizar la tesis (julio de 2018) cuando empecé a programar más intensamente en `R`, así que se podría decir que es el lenguaje que menos horas he dedicado (pero en el que más he producido, curiosamente). Y es que mientras que **`Python` es un lenguaje de un propósito mucho más general**, **`R` fue diseñado por y para matemáticos y estadísticos**, y se nota desde la propia arquitectura del lenguaje. Obviamente este objetivo tan específico tiene una desventaja: por regla general, **`Python` es más eficiente** (con tiempos de ejecución más cortos), y está dotado de una **mayor flexibilidad** para el desarrollo web, la Inteligencia Artificial, el preprocesamiento de imágenes o la integración con todo tipo de apps o programas (incluso con herramientas de edición de audio y vídeo de la saga Adobe).

Ambos tienen **tres ventajas** que los hacen muy difícil de superar en el ámbito del análisis de datos:

* **Software libre**, con una **inmensa comunidad de usuarios** produciendo y validando código: seguramente lo que necesites ya haya sido implementado (en su totalidad o de forma parcial) por alguien antes y solo necesites adaptarlo.

* **Fácil integración de otros lenguajes**, como puede ser `FORTRAN` o `C++`, para tareas más tediosas y costosas (como la programación en paralelo).

* **Modulares**: su instalación básica ocupa muy poco espacio, y mediante la instalación de paquetes (`R`) o librerías (`Python`), permiten su configuración totalmente adaptada a nuestras necesidades.


Dada su flexibilidad y potencia, ambos seguramente cubran tus necesidades en cuanto a análisis de datos se refiere, por lo que si ya has empezado con alguno de ellos, mi **consejo es que sigas con el lenguaje que te resulte más cómodo, y del que tengas ya cierta base**. Sin embargo, si **estás partiendo de cero**, mi recomendación (para el análisis de datos) es sin duda `R` ya que cuenta con tres ventajas frente a `Python`:

* En lo referente al análisis de datos y la estadística, **`R` cuenta una mayor comunidad de usuarios**, por lo que tendrás a tu disposición una mayor variedad de paquetes y de soporte en la web.
* Fue diseñado especialmente para el análisis de datos, por lo que se requieren **muy pocas líneas de código** para la implementación de flujos de trabajo en la carga de datos, preprocesamiento, modelos predictivos y validación.
* La **gran fortaleza de `R`** es contar con **herramientas muy potentes para la visualización de datos** (como el paquete `{ggplot2}`) y la presentación de resultados (como los paquetes `{shiny}` para crear apps interactivas con el usuario, `{bookdown}` para crear libros con código y latex integrado, o `{blogdown}` para crear webs como en la que estás).


Es por todo ello por lo que **mi recomendación si estás empezando en el análisis estadístico**, o el uso que le vas a dar está orientado a la **producción de informes** o análisis estadísticos para revistas científicas, sea apostar por `R` pero sin volverte loco/a: si ya tienes conocimientos de `Python` y/o la mayor parte de tus colegas de profesión lo están usando, mi consejo es que sigas apostando por él.

* Tutorial para muggles: [primeros pasos en `R`](https://aprendiendo-r-intro.netlify.app/)

| Lenguaje | Ventajas | Desventajas |
|----------|-------------|------|
| Matlab   | gran cantidad de herramientas en las toolbox - cálculo matricial - modelado 3D | software de pago - alto consumo de memoria - lento - propósito demasiado general|
| R        | software libre - pensado por y para la estadística - gran cantidad de usuarios y paquetes disponibles - visualización y análisis de datos - creación de informes con código integrado |  mayor dificultad para el desarrollo web - mal programado puede ser lento |
| Python   | rápido - software libre - facilidad en lectura de archivos - integración sencilla con otros lenguajes y aplicaciones - Inteligencia Artificial - preprocesamiento de imágenes | Problemas en el manejo de grandes bases de datos - no orientado especificamente al análisis y visualización estadística |





&nbsp;

## Breve y cutre cronología de los lenguajes de programación {#cronologia}

* **1843**. Aunque el mérito cinematográfico se lo llevó Alan Turing, fue una mujer, **Ada Lovelace**, la primera en crear lo que hoy llamaríamos un algoritmo computacional mecánico: una secuencia finita de pasos realizados por una maquina (en este caso, un telar).

* **1936**. Apoyándose en las ideas de Lovelace, **Turing** diseñó una máquina capaz de almacenar datos en una cinta y procesas los símbolos guardados en ella siguiendo una colección de reglas lógicas.

* **1944**. Coincidiendo con el final de la Segunda Guerra Mundial, empezaron a aparecer las primeras computadoras alimentadas con electricidad, siendo Konrad Zuse el desarrollador del primer lenguaje de programación moderno, `Plankalkül`, proporcionando procedimientos para guardar pedazos de código y así poder realizar de forma sistemática operaciones rutinarias.

* **1949**. Nace el **lenguaje ensamblador**, el lenguaje de programación de más bajo nivel, el conjunto de reglas más sencillo para dar instrucciones a componentes electrónicos.

* **1957**. Nace `FORTRAN`, probablemente el lenguaje de programación más importante de la historia de la informática y el más antiguo que sigue aún en uso. Aunque sigue siendo un lenguaje de bajo nivel (tiempos elevados en su programación, tiempos muy reducidos en su ejecución y compilación), `FORTRAN` permite la realización de cálculos matemáticos y estadísticos de gran complejidad.

* **1964-1970**. Nacen `BASIC` y `PASCAL`, los primeros lenguajes de programación orientados a estudiantes de ciencias que no tuvieran grandes conocimientos de informática y fáciles de aprender, razones por las que fueron los lenguajes por los que apostaron en un primer momento Microsoft y Apple, respectivamente.

* **1972**. IBM lanzó `SQL` (otrora SEQUEL), el lenguaje de programación más importante el manejo de bases de datos y la base de la mayoría de sistemas de gestión de datos, permitiendo una consulta muy eficiente de ficheros.

* **1972-1983**. Los desarrolladores de los laboratorios de la Bell Telephone lanzan `C`, junto con `FORTRAN` el lenguaje de programación más importante y usado, en el que posteriormente se han basado lenguajes como `C#`, `Java`, `JavaScript`, `Perl`, `PHP` o `Python`. En 1983 Bjarne Stroustrup extendió dicho lenguaje derivando en `C++`, el lenguaje motor de herramientas como Office, Adobe o algunos videojuegos.


* **1976**. Los laboratorios Bell sacaron la primera versión del lenguaje conocido `S`, un primer intento de lenguaje de programación enfocado al análisis estadístico y el cálculo matemático.

* **1991**. Inspirados en los Monty Python, Guido Van Rossum desarrolló `Python`, un lenguaje libre, de alto nivel, modaular y con un propósito general, siendo el lenguaje por el que han apostado empresas como Spotify o Netflix.

* **1993**. Expertos en estadística computacional (el conocido como R Development Core Team) decidieron apostar por extender `S` a `R`, para obtener un lenguaje de programación más estable y de licencia gratuita.


 
* **1995**. James Gosling crea `Java`, el lenguaje orientado a objetos más importante y en el que se basan otros lenguajes posteriores, con el objetivo de desarrollar herramientas y softwares interactivos con el usuario.




