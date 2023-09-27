# Ordenamiento por incrementos decrecientes (Shell)

El ordenamiento por incrementos decrecientes, también conocido como ordenamiento de Shell, es un algoritmo de ordenamiento que combina el ordenamiento por inserción con una técnica de divide y vencerás para aumentar la eficiencia. El algoritmo funciona dividiendo el arreglo en subarreglos más pequeños y luego ordenándolos individualmente antes de combinarlos en un solo arreglo ordenado.

Aquí hay un ejemplo de código de ordenamiento por incrementos decrecientes en C#:

```csharp
using System;

int[] arr = { 5, 2, 9, 1, 5, 6 };
Console.WriteLine("Arreglo desordenado:");
PrintArray(arr);

ShellSort(arr);

Console.WriteLine("Arreglo ordenado:");
PrintArray(arr);

static void ShellSort(int[] arr)
{
    int n = arr.Length;
    int gap = n / 2;

    while (gap > 0)
    {
        for (int i = gap; i < n; i++)
        {
            int temp = arr[i];
            int j;
            for (j = i; j >= gap && arr[j - gap] > temp; j -= gap)
                arr[j] = arr[j - gap];
            arr[j] = temp;
        }
        gap /= 2;
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

> En este ejemplo, el método `ShellSort` recibe un arreglo de enteros y los ordena utilizando el algoritmo de ordenamiento por incrementos decrecientes. Después de ordenar el arreglo, se imprime en pantalla tanto el arreglo desordenado como el arreglo ordenado.
>