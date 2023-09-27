La búsqueda secuencial es un algoritmo de búsqueda simple que consiste en recorrer una lista elemento por elemento hasta encontrar el elemento que se está buscando. Si se encuentra el elemento, se devuelve su índice. Si no se encuentra, se devuelve un valor indicando que el elemento no está presente en la lista.

Aquí hay un ejemplo de código de búsqueda secuencial en C#:

```csharp
using System;
int[] arr = { 5, 2, 9, 1, 5, 6 };
Console.WriteLine("Arreglo: ");
PrintArray(arr);

Console.WriteLine("Ingrese un número a buscar: ");
int number = int.Parse(Console.ReadLine());

int index = SequentialSearch(arr, number);
if (index == -1)
{
    Console.WriteLine("El número no se encuentra en el arreglo.");
}
else
{
    Console.WriteLine("El número se encuentra en el índice " + index + " del arreglo.");
}

static int SequentialSearch(int[] arr, int number)
{
    for (int i = 0; i < arr.Length; i++)
    {
        if (arr[i] == number)
        {
            return i;
        }
    }
    return -1;
}

static void PrintArray(int[] arr)
{
    for (int i = 0; i < arr.Length; i++)
    {
        Console.Write(arr[i] + " ");
    }
    Console.WriteLine();
}
```

> En este ejemplo, el método `SequentialSearch` recibe un arreglo de enteros y un número, y devuelve el índice del número en el arreglo si se encuentra, o un valor indicando que el número no está presente en el arreglo. Después de buscar el número, se imprime en pantalla el resultado de la búsqueda.
>