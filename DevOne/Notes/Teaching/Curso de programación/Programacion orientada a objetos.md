El paradigma de programacion orientada a objetos es una parte fundamental de cualquier desarrollador, dado que, en algun punto de su carrera hara uso de este paradigma.

Es el paradigma mas popular de todos, aunque, no necesariamente el mejor, existen diferentes paradigmas orientados a diferentes problemas, es decision del desarrollador decidir que paradigma utilizar para solucionar el problema que se le presente.

Este paradigma hace uso de conceptos como **clases** y **objetos**. Las clases se utilizan para crear piezas de codigo reutilizables, similar a los planos de construccion, que pueden ser utilizadas para despues crear objetos a partir de esos planos.

Por ejemplo, una clase podria definirse de la siguiente forma.

```json
La clase Automovil tiene dos atributos, color y marca.
```

Para despues crear un objeto concreto como este

```json
El objeto Focus es un Automovil, tiene color rojo y marca Ford.
```

Las clases definen que propiedades van a portar los objetos que se van a derivar de ellas, pero no los valores que contendran esos objetos.

Las clases tambien pueden definir el comportamiento de esos objetos, por ejemplo:

```json
A la clase Automovil le es posible Acelerar y Frenar.
```

Para que despues un objeto defina esos comportamientos:

```json
El objeto Focus de tipo Automovil le es posible Acelerar a un maximo de 120 km/h y Frenar dependiendo de la velocidad alcanzada.
```

Existen 4 principios de la programacion orientada a objetos, la herencia, abstraccion, el encapsulamiento y el polimorfismo, los veremos mas adelante.