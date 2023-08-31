# Principios de prevención de defectos 2
Materia: Computación Tolerante a Fallas<br>
Maestro: MICHEL EMANUEL LOPEZ FRANCO<br>
Nombre: Diego Alonso Mercado Brizuela<br>
Carrera: Ingeniería en Computación<br>
Código: 215425636<br>
Fecha: 31/08/2023<br>
Sección: D06<br>

## Introducción
La prevención de errores es un método para poder combatir los errores en fase de desarrollo o ya en la producción del mismo producto, por lo que ayudaría de gran medida a que no aparezcan errores o por lo menos disminuir parte de ellos. Si uno desea un sistema de software de alta calidad, uno debe asegurarse de que cada una de sus partes sea de alta calidad. Al mejorar la administración de los defectos, uno producirá componentes de software más confiables. Por lo tanto, para mejorar la calidad del
producto, debe mejorarse la calidad del proceso.
## Clasificación ortogonal de defectos
Se trata de un esquema desarrollado por IBM para clasificar defectos con el fin de proveer retroalimentación sobre el progreso de un proyecto, a través del mismo. El objetivo de su creación es obtener un paradigma para medir las relaciones causa-efecto de los defectos, donde se pudiera encontrar la causa raíz de un defecto. Al mismo tiempo se deseaba desarrollar una clasificación de defectos que fuera simple y que estuviera lo más libre posible de errores humanos.
A partir de las investigaciones que permitieran obtener esta clasificación se demostró que al clasificar de forma única los defectos utilizando un conjunto de tipos de defectos que reflejaran la semántica de las reparaciones hechas, se puede asociar los tipos de defectos con las fases de desarrollo. 
ODC significa esencialmente que se clasifica a un defecto en uno de varios posibles tipos,
los cuales apuntan a la parte del proceso que necesita atención.
Para esto se agregó dos atributos a los defectos: tipo de defecto y desencadenador (trigger) de un defecto.
El tipo de defecto clasifica a un éste a través de la semántica de la reparación que se
necesitó hacer para remover al defecto del sistema. La selección del tipo de defecto se
deriva de la corrección hecha por el desarrollador. Para cada uno de estos tipos, el
desarrollador también indica si el defecto consiste en que la información en el componente hace falta, o si es incorrecta. 
Los tipos de defectos definidos son:
- Función. Afecta las interfaces de usuario, las interfaces del producto, las interfaces con
el hardware, y las estructuras de datos. Requiere un cambio formal en el diseño.
- Asignación. Generalmente indica errores en el código, al inicializar o asignar valores de
variables o estructuras de datos. 
- Interfase. Se refiere a errores en las interacciones entre componentes, módulos u otros
dispositivos a través de las llamadas a funciones, paso de parámetros, etc.
- Chequeo. Errores en la lógica del programa, el cual no hace la verificación de los datos
y valores antes de ser usados.
- Serialización/temporal. Errores que tienen que ver con los recursos compartidos y de
tiempo real.
- Construcción/Empaquetado (Build/Package/Merge). Errores que ocurren debido a
problemas en las librerías, así como problemas en el control de cambios y versiones.
- Documentación. Errores que pueden afectar a la documentación de los artefactos o al
mantenimiento del sistema.
- Algoritmo. Problemas de eficiencia o corrección de una tarea, a través del algoritmo
que define a esa tarea. 
Los tipos de defectos deben ser ortogonales, es decir, que son mutuamente excluyentes.
Esto asegura que al encontrarse un defecto, este será solamente de un tipo posible, y no
podrá caerse en la situación de clasificar incorrectamente a un defecto, ya que no será
posible clasificar a un defecto en dos posibles tipos. Al mismo tiempo, los tipos de defectos definidos deben cubrir todas las posibles ocurrencias de los defectos en un sistema, de manera que ningún defecto pueda quedar sin clasificación.
El objetivo de los tipos de defectos también es poder relacionar cada tipo con algunas de las fases del proceso de desarrollo. Se trata de determinar dónde fueron inyectados los defectos en el sistema. Se encontró que cada tipo de defecto tiende a ser inyectado en relativamente pocas áreas o fases de desarrollo. Por ejemplo, los defectos de asignación tienden a ser inyectados en su mayoría en la fase de codificación, y los defectos de algoritmo tienden a ser inyectados especialmente en la fase de diseño de bajo nivel. 
# Conclusiones
Este método de clasificación ayudaría mucho a la industria porque haría más eficiente la detección de errores, que es lo que se quiere evitar hoy en día, los errores que a todo programador le pasan, por lo que implementar este método en nuestros proyectos será fundamental
