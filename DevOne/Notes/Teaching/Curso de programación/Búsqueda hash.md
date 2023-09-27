La búsqueda hash es un algoritmo de búsqueda que utiliza una función hash para calcular un índice para cada elemento en un arreglo. La función hash asigna un valor único a cada elemento basado en su valor. De esta manera, se puede acceder a un elemento directamente en el arreglo sin tener que buscar secuencialmente a través de todo el arreglo.

Aquí hay un ejemplo de código de búsqueda hash en C#:

```csharp
using System;
using System.Collections.Generic;

Dictionary<int, string> hashTable = new Dictionary<int, string>();
hashTable.Add(1, "Alice");
hashTable.Add(2, "Bob");
hashTable.Add(3, "Charlie");
hashTable.Add(4, "David");
hashTable.Add(5, "Eve");

Console.WriteLine("Tabla hash: ");
PrintHashTable(hashTable);

Console.WriteLine("Ingrese una clave a buscar: ");
int key = int.Parse(Console.ReadLine());

string value;
if (hashTable.TryGetValue(key, out value))
{
    Console.WriteLine("Valor asociado a la clave " + key + ": " + value);
}
else
{
    Console.WriteLine("No se encontró ningún valor asociado a la clave " + key + ".");
}

static void PrintHashTable(Dictionary<int, string> hashTable)
{
    foreach (KeyValuePair<int, string> entry in hashTable)
    {
        Console.WriteLine("Clave: " + entry.Key + ", Valor: " + entry.Value);
    }
}

```

> En este ejemplo, se utiliza una clase `Dictionary` para almacenar los elementos y sus claves en una tabla hash. El método `TryGetValue` se utiliza para buscar un elemento en la tabla hash mediante su clave y devolver su valor si se encuentra. Después de buscar un elemento, se imprime en pantalla el resultado de la búsqueda.
>