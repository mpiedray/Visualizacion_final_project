# Creación de la visualización y entrega del proyecto (Práctica)

Como ya comentamos en la práctica anterior, la seleccion de este dataset a sido por motivos personales, a raiz de la cumbre sobre el clima organizada por Naciones Unidas en Glasgow(Escocia), donde habian grandes promesas para salvar al planeta pero que en realidad al final del evento los grandes compromisos han sido pocos y se sacaron con bastante dificultad.

Para la realización de esta práctica tuve que leer y refrescar sobre algunos conceptos y terminos finacieros para poder entender los datos con los que iba a trabajar.

Por ul lado tenemos el GDP (gross domestic product) o el PIB (producto interior bruto)
el PIB de calcula como:

` PIB = C + I + G + (X-M)`

El PIB lo podemos desglosar en:

- PIB nominal o PIB precio corriente: es aquel que **no esta ajustado** por los efectos de la inflación y a los precios corrientes del mercado.

- PIB real o PIB precio constante: es el que **esta ajustado** por los efectos de la inflaccion.

> El PIB a precio constante es menor que el PIB corriente y es la medida mas precisa para conecer el estado de un pais, ya que la inflaccion disminuye el valor temporal del dinero y reduce la cantidad de bienes y servicios que se puedan comprar en un futuro. 

Por otro lado tenemos el índice de Desarrollo Humano (IDH) es un indicador nacido de la mano del Programa de Naciones Unidas para el Desarrollo (PNUD) que sirve para evaluar cómo de desarrollada está una sociedad. Este indice esta basado en tres dimensiones principales: esperanza de vida, educación y riqueza económica.

Se entiende por desarrollo humano el proceso por el que pasa una sociedad cuando en ésta hay mejoras en las condiciones de vida de sus ciudadanos. Estas mejoras no únicamente implican un incremento en los bienes de los que disponen, los cuales, indudablemente, les van a ayudar a satisfacer sus necesidades básicas como pueden ser alimentación, vivienda y transporte, tambien implica la creacion de un entorno en el que se respeten los derechos humanos de todos y cada uno de los ciudadanos residentes en el país, su derecho a la educación y al tener una vida digna. 

**Un mayor desarrollo humano puede entenderse como sinónimo de un alto grado de libertad y cantidad de opciones que se dispongan para ser o hacer lo que se desee.**

Para calcular el índice de dimensión de cada caso en concreto es decir en esperanza de vida , educacion y riqueza economica se usa la siguiente formula:

`Índice de dimensión = (valor actual – valor mínimo) / (valor máximo – valor mínimo)`

* **Esperanza de vida:**
  + El valor mínimo 20 años.
  + Valor máximo 85 años.


* **Educación:**
  + El valor mínimo 0 años.
  + Valor máximo esta esta en 18 años. (equivalente a haber obtenido una titulación universitaria).
  + La escolarización media fija su máximo en 15 años.


* **PIB per cápita:**
  + La cifra mínima en 100 dólares.
  + La cifra máximo en 75.000 dólares.

El valor máximo se ha fijado en 75.000 dólares porque se ha visto que no existen ganancias significativamente diferente en el desarrollo humano y el bienestar cuando el PIB supera esa cifra.

Una vez calculados los índices de cada dimensión, se realiza el cálculo del Índice de Desarrollo Humano en sí, usando la siguiente fórmula:

`IDH = (Índice de Salud X Índice de Educación X Índice de Ingreso)^⅓`

Si un país tiene el máximo en todo, su IDH es de 1, lo cual significa que tiene un elevadísimo nivel de desarollo. En cambio, si tiene mínimos en todo, su IDH será de 0.

***

**1. El proceso de creación que se siguió y decisiones de diseño que se han tomado a lo largo del desarrollo.**

En mi caso comence con el diseño visualizando un mapa, para usarlo como filtro, para poder ir filtrando por paises las caracteristicas que queria destacar, finalmente opte por quitar el mapa y seguir filtrando por paises usando un selector, ya que a la hora de crear un dashboard el mapa ocupaba demasiado espacio para usarlo solo como filtro, de hecho valore la posibilidad de poner informacion sobre el pero iagualmente no me convencio, ya que al haber mas elementos en el dashboard el mapa se mostraba pequeño para mostrar información sobre el.

Finalmente mi visualización esta formada por tres dashboard unidos todos con enlaces para poder ir saltando de uno a otro. He dividido las visualizacion por temas, en mi caso dos:
- Salud: Donde se responbde a a las preguntsa sde inmunizacion de la poblacion, acceso a agua potable y demas, aspectos de mortalidad infantil, etc.

- Educacion y Empleo: Donde se responden a las preguntas de tasas de desempleo, educación en cuanto a paises, etc.

Cada uno de los temas es un dashboard y el tercero es el dashboard principal desde donde se puede acceder al resto.

**2. La presentación in situ de la visualización, es decir, comentar sobre las características de la visualización mientras navega.**

Se explica en el video.

**3. El conjunto de datos que se muestran.**

He usado los datos que seleccione en la práctica 1, si bien es cierto que nos lo use todos porque el dataset era bastante extenso, en este caso use los relacionados con temas de salud, educación y empleo, que cubren la mayoría de las preguntas planteadas.

Previo a empezar a crear la visualizacion tuve que tratar  los datos, de manera que pudieran ser entendidos por la aplicacion que iba a usar, en este caso Tableau Public

**4. Las preguntas que contengan la vista.**

1. ¿Se ha conseguido disminuir la brecha salarial entre hombres y mujeres?

2. ¿Ha disminuido la desigualda social entre hombres y mujeres (tanto para paises desarrollas como los que no?

3. ¿Se ha aumentado la presencia femenina a la hora de obtener educación?

4. ¿Como ha variado el ausentismos en los colegios a todos los niveles?

6. ¿Como ha variado en todos los paises los niveles de vacuanacion en ninos y adolescentes? 

**5. Los elementos interactivos disponibles como parte de la pantalla.**

En nuestra visualización tenemos varios elementos de navegación y composición que nos permiten estudiar los datos. Por un lado tenemos colores, usando el rojo para aspectos femeninos y el azul para aspectos  masculinos, lo cual nos es mas facil de leer visualmente, ya que estamos acostumbrados a esos colores a la hora de hablar de genero.

También tenemos filtros que nos dejan en este caso elegir por paises, para poder comparar unos con otros y asi ver las diferencias.
Cabe destacar que al modificar el filtro del país cambia completamente el dashboard, ya que cada elemento esta relacionado con ese filtro y toda la información que se muestra es relacionada con el país seleccionado.

Por ultimos tenemos enlaces o link en cada dashboard que nos permiten movernos por los diferentes dashoard.
