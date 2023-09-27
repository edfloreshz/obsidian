# Ordenamiento por inserción

El ordenamiento por inserción es un algoritmo de ordenamiento simple que funciona comparando y colocando cada elemento en su posición correcta en una lista o arreglo desordenado. Es un algoritmo eficiente para arreglos pequeños o arreglos que ya están parcialmente ordenados.

Aquí hay un ejemplo de código de ordenamiento por inserción en C#:

```csharp
using System;

int[] arr = { 5, 2, 9, 1, 5, 6 };
Console.WriteLine("Arreglo desordenado:");
PrintArray(arr);

InsertionSort(arr);

Console.WriteLine("Arreglo ordenado:");
PrintArray(arr);

static void InsertionSort(int[] arr)
{
    for (int i = 1; i < arr.Length; i++)
    {
        int current = arr[i];
        int j = i - 1;
        while (j >= 0 && arr[j] > current)
        {
            arr[j + 1] = arr[j];
            j--;
        }
        arr[j + 1] = current;
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

> En este ejemplo, el método `InsertionSort` recibe un arreglo de enteros y los ordena utilizando el algoritmo de ordenamiento por inserción. Después de ordenar el arreglo, se imprime en pantalla tanto el arreglo desordenado como el arreglo ordenado.
>