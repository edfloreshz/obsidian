# Expresiones

Una expresión es una pieza de código que al resolverse, da como resultado un valor.

```csharp
var resultado = a + b * c;
```

## Tipos de expresiones

### Expresiones constantes

Consisten solamente de valores constantes.

```csharp
5 + 10
```

### Expresiones integrales

Estas expresiones producen valores de tipo numero entero.

```csharp
var x = 1;
var y = 2;

x * y // 2
```

### Expresiones flotantes

Estas expresiones producen valores de tipo numero flotante.

```csharp
10.75 + 4.20 // 14.95
```

### Expresiones relacionales

Estas expresiones hacen uso de operadores relacionales como `<` `>` `<=` `>=`, entre otros, y producen resultados de tipo booleanos, es decir, verdadero o falso.

```csharp
10 > 4 // verdadero
10 > 20 // falso
10 >= 10 // verdadero
```

### Expresiones lógicas

Estas expresiones combina dos o mas expresiones relacionales, y haciendo uso del algebra booleana, producen resultados de tipo booleano.

```csharp
var x = 10;
var y = 5;

x > y && x == 10 // verdadero
x == 10 || y == 5 // verdadero
```