Es posible declarar tipos de datos con otros nombres, esto puede hacer que nuestro código sea mas entendible.

```csharp
using ListaDeClientes = System.Collections.Generic.List<Cliente>;

ListaDeClientes lista = new();
```

Sin embargo, se recomienda no crear tipos personalizados para tipos de datos ya existentes:

```csharp
using IntegerType = int;
using StringType = string;
using BooleanType = bool;
```

Dado a que es innecesario y puede crear confusion en otros programadores.