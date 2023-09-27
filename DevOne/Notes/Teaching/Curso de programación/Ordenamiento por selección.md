# Ordenamiento por selección

El ordenamiento por selección es un algoritmo de ordenamiento simple que funciona seleccionando el elemento mínimo de una lista y intercambiándolo con el primer elemento no ordenado. Luego, se repite este proceso para cada elemento no ordenado hasta que toda la lista esté ordenada.

Aquí hay un ejemplo de código de ordenamiento por selección en C#:

```csharp
using System;

int[] arr = { 5, 2, 9, 1, 5, 6 };
Console.WriteLine("Arreglo desordenado:");
PrintArray(arr);

SelectionSort(arr);

Console.WriteLine("Arreglo ordenado:");
PrintArray(arr);

static void SelectionSort(int[] arr)
{
    for (int i = 0; i < arr.Length - 1; i++)
    {
        int minIndex = i;
        for (int j = i + 1; j < arr.Length; j++)
        {
            if (arr[j] < arr[minIndex])
            {
                minIndex = j;
            }
        }

        int temp = arr[minIndex];
        arr[minIndex] = arr[i];
        arr[i] = temp;
    }
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

> En este ejemplo, el método `SelectionSort` recibe un arreglo de enteros y los ordena utilizando el algoritmo de ordenamiento por selección. Después de ordenar el arreglo, se imprime en pantalla tanto el arreglo desordenado como el arreglo ordenado.
>