Las enumeraciones son un tipo especial que representa un grupo de constantes, de modo que no son modificables. 

Son comúnmente utilizadas para representar opciones de las cuales se puede elegir, como el día de la semana:

```csharp
enum Dias {
	Lunes,
	Martes,
	Miercoles,
	Jueves,
	Viernes,
	Sabado,
	Domingo
}
```

Por defecto, las enumeraciones se numeran automáticamente de cero en adelante cuando se declaran, el lenguaje termina con un código como este:

```csharp
enum Dias {
	Lunes = 0,
	Martes = 1,
	Miercoles = 2,
	Jueves = 3,
	Viernes = 4,
	Sabado = 5,
	Domingo = 6
}
```

Sin embargo, es posible modificar el valor que se le asigna a cada constante de la enumeración.

```csharp
enum Dias {
	Lunes = 7,
	Martes = 6,
	Miercoles = 5,
	Jueves = 4,
	Viernes = 3,
	Sabado = 2,
	Domingo = 1
}
```