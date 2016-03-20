# Guía para la resolución de problemas y un mejor entendimiento de Classical Electrodynamics de John David Jackson.

**Para comenzar digo que no me considero un experto, ni mucho menos, en el tema de electrodinámica, pero espero que este repositorio ayude a más de uno en su vida académica y profesional.**

Como estudiante de Licenciatura en Física, y ahora Maestría en Física, me he encontrado varias veces el problema que significa resolver los problemas de Classical Electrodynamics de Jackson, o "el Jackson". En este repositorio pienso agregar la mayor cantidad de información posible la cual debería facilitar la solución de los problemas del texto, así como un mejor entendimiento del mismo. El repositorio consistirá de tareas, tanto propias como de otros estudiantes, así como tareas que encuentre en internet, también de complementos al texto, soluciones aisladas y cualquier otra información que pueda ser relevante.

Comienzo traduciendo la introducción al solucionario del texto, que se puede encontrar [aquí](http://libgen.io/book/index.php?md5=DDE50D8F541CF943072C07366E33EA45). 

# Traducción de la introducción al solucionario de Jackson.

Debido a que ciertas ramas de las matemáticas son usadas con fluidez en electrodinámica clásica, una corta lista de las funciones más usadas y matemática debe ser presentada antes de discutir la solución a los problemas.

El análisis vectorial y tensorial son prerequisitos debido a que los campos eléctricos y magnéticos pueden ser derivados  
tanto de un potencial escalar como de uno vectorial. El gradiente, la divergencia, el rotacional y el operador de Laplace forman la columna vertebral de la electricidad y el magnetismo. Las soluciones del potencial son representadas usualmente mediante expansiones ortogonales, cuyos coeficientes de la expansión pueden obtenerse haciendo uso de las propiedades de la ortogonalidad. Las expansión en series de Fourier es una de ese tipo. Coordenadas adecuadas deben ser escogidas para simetrías particulares del problema. Aunque puede ser ventajoso conocer coordenadas elípticas y coordenadas generalizadas, no aparecen a menudo en este libro. La función delta de Dirac es usada para describir la posición de las cargas discretas 
en vez de una distribución de carga en la integración. El plano complejo para el mapeo conforme, integración residual en soluciones retardadas debido a la velocidad finita de la luz y la corta duración de la fuenta, y las funciones de Green son unaos de los acercamientos generales para obtener el potencial. Electrodinámica Clásica por Jackson ofrece una discusión 
general de las matemáticas cuando es requerido, lo cual comúnmente es suficiente para manejar los problemas.

El énfasis de este resumen es primeramente sobre los métodos para solucionar los problemas. La primera parte describe electrostática y magnetostática. Las técnicas para resolver problemas de electrostática en el libro son:

(1) Ley de Coulomb: Es un acercamiento básico pero poco conveniente. 

![Ecuación 1](https://github.com/FavioVazquez/Guia-Jackson-Electrodinamica/blob/master/Images/ec1.gif)

Debido a las cantidades vectoriales **F** y **E**, la mayoría de los problemas son resueltos mediante potenciales. 

(2) Potencial: Para el caso electrostático **&nabla;**	x **E** = 0, por lo tanto la intensidad de campo eléctrico **E** puede expresarse en términos de un potencial **E** = -**&nabla;** &Phi;. El potencial &Phi; es una cantidad escalar, por lo que la superposición es la suma escalar de las contribuciones individuales de cada una de las fuentes de las distribuciones de carga. Varios métodos son utilizados en problemas de potencial, como 

  (a) Ley de Gauss: Es una consideración general de una superficie cerrada y distribución de carga adentro de un volumen encerrado. La forma integral de la ley de Gauss es

![Ecuación 2](https://github.com/FavioVazquez/Guia-Jackson-Electrodinamica/blob/master/Images/ec2.gif)

y su forma diferencial equivalente es

![Ecuación 3](https://github.com/FavioVazquez/Guia-Jackson-Electrodinamica/blob/master/Images/ec3.gif)

Para un problema simple, si la superdficie gaussiana es construida de acuerdo a la geometría delproblema, entonces el problema está resuelto. De otra manera, la ley de Gauss lleva a la ecuación de Laplace (&nabla;<sup>2</sup> &Phi; = 0) o a la ecuación de Poisson (&nabla; &Phi; = -4 &pi; &rho;), que sirve cono punto de comienzo para la mayotía de los problemas. El operador de Laplace es dependiente de la geometría. Las funciones especiales con los sistemas de coordenadas son los siguientes:

(i) Coordenadas Cartesianas: Expansiones ortogonales de las funciones seno y coseno.
(ii) Coordenadas Cilíndricas: Funciones de Bessel (J<sub>l</sub>).
(iii) Coordenadas Esféricas: Polinomios de Legendre (P<sub>l</sub>), polimonios de Legendre asociados (P<sub>l</sub><sup>m</sup>), esféricos armónicos (Y<sub>lm</sub>) y funciones esféricas de Bessel (j<sub>l</sub>).

(b) Expensión multipolar: Es comúmmente el método más usado en problemas de electrostática y electrodinámica. Mediante una expansión directa de Taylor del potencial &Phi;, da el monopolo (&rho;) dipolo (momento dipolar) y cuadrupolo (momento cuadrupolar) y términos sde orden superior en x o momentos multipolares de orden superior.

(c) Función de Green G(**x**,**x**'): También es un método general para encontrar la solución al problema. Es deducida del teorema de Green.

![Ecuación 4](https://github.com/FavioVazquez/Guia-Jackson-Electrodinamica/blob/master/Images/ec4.gif)

Reemplazando el potencial &Phi; por &phi; y G (función de Green) para &psi;, entonces, 

![Ecuación 5](https://github.com/FavioVazquez/Guia-Jackson-Electrodinamica/blob/master/Images/ec5.gif)

La función de Green solo depende de **x**' (el vector de desplaznamiento desde el origen a la distribución de carga) y **x** (el vector de desplazamiento desde el origen al punto de observación). Usando las condiciones de frontera para eliminar uno de los términos en los corchetes (i.e. condiciones de frontera de Dirichlet o Neumann), esto es esquivalente al potencial de una carga unitaria y es simétrico con respecto a **x** y **x**' (es decir que intercambiar **x** y **x**' no altera el efecto total del potencial).

(3) Método de las imágenes: Simplifica el problema en gran parte, sin embargo su aplicación está limitada a geometrías simples de problemas como cargas y una placa conductura infinita con un potencial constante; dos placas conductoras paralelas, con cargas en el medio; una carga y una esfera con potencial constante o carga añadida, etc.

Las imágenes (magnitudes y posiciones) simulan las mismas condiciones de frontera especificadas por la placa conductora, la esfera, etc., luego se ser removidas. Sin embargo, el potecial calculado solo sirve para representar la región donde las cargas reales están situadas y está ligado a las placas conductoras, esfera, etc. Para tratar zonas fuera de esta región, debe tenerse mucho cuidado. Esto importa cuando tratamos problemas con dieléctricos, ya que el potencial adentro y afuera del medio dieléctrico son interesantes. 


