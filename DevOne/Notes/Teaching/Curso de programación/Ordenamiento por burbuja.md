El ordenamiento por intercambio, también conocido como ordenamiento por burbuja, es un algoritmo de ordenamiento sencillo y eficiente para arreglos pequeños. El algoritmo funciona comparando cada par de elementos adyacentes y intercambiándolos si están en el orden incorrecto. Este proceso se repite hasta que el arreglo esté ordenado completamente.

Aquí hay un ejemplo de código de ordenamiento por intercambio en C#:

```csharp
using System;

int[] arr = { 5, 2, 9, 1, 5, 6 };
Console.WriteLine("Arreglo desordenado:");
PrintArray(arr);

BubbleSort(arr);

Console.WriteLine("Arreglo ordenado:");
PrintArray(arr);

static void BubbleSort(int[] arr)
{
    int n = arr.Length;
    for (int i = 0; i < n - 1; i++)
    {
        for (int j = 0; j < n - i - 1; j++)
        {
            if (arr[j] > arr[j + 1])
            {
                int temp = arr[j];
                arr[j] = arr[j + 1];
                arr[j + 1] = temp;
            }
        }
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

> En este ejemplo, el método `BubbleSort` recibe un arreglo de enteros y los ordena utilizando el algoritmo de ordenamiento por intercambio. Después de ordenar el arreglo, se imprime en pantalla tanto el arreglo desordenado como el arreglo ordenado.
>