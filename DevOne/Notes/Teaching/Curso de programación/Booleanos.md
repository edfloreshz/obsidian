El tipo de dato `bool` representa un valor de `true` o `false`. Para hacer uso de estos operadores, se utilizan operadores de lógica booleana.

Se puede utilizar `true` o `false` para inicializar variables.

```csharp
bool estaLloviendo = true;

bool a = true || false || true; // true
bool b = true && true && true; // true

bool llovio = estaLloviendo;
bool llovio = !estaLloviendo;
```

Se pueden evaluar las expresiones de tipo `bool` de la siguiente forma:

```csharp
Console.WriteLine(estaLloviendo ? "Esta lloviendo!" : "No esta lloviendo...");
```

Lo cual seria equivalente a el siguiente código:

```csharp
if (estaLloviendo) {
	Console.WriteLine("Esta lloviendo!");
} else {
	Console.WriteLine("No esta lloviendo...");
}
```

Si la variable `estaLloviendo` es verdadera, se imprime `“Esta lloviendo!”`, si no, imprime `"No esta lloviendo..."`.