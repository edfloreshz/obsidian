Cada variable tiene un alcance, esto significa que una vez que el programa alcanza el final de ese alcance, esa variable se elimina de la memoria. 

```csharp
{ // Este es el inicio del programa.

	// La variable nombre se crea aqui, por lo tanto, su alcance comienza aqui.
	var nombre = "Julian"; 

	// Aqui se hace uso de la variable, por lo tanto, aun no hemos llegado al final de su alcance.
	print(nombre); 

} // Este es el final del alcance de la variable nombre.
```