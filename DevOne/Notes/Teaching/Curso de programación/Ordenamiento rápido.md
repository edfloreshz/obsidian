# Ordenamiento rápido

El ordenamiento rápido, también conocido como QuickSort, es un algoritmo de ordenamiento eficiente y rápido que es adecuado para arreglos de tamaño moderado a grande. Funciona eligiendo un elemento de pivote y reordenando los elementos restantes en torno a él, de tal manera que los elementos menores que el pivote se encuentren a la izquierda y los elementos mayores a la derecha. Luego, se aplica este mismo proceso a las sublistas resultantes recursivamente hasta que se hayan ordenado todos los elementos.

Aquí hay un ejemplo de código de ordenamiento rápido en C#:

```csharp
using System;

int[] arr = { 5, 2, 9, 1, 5, 6 };
Console.WriteLine("Arreglo desordenado:");
PrintArray(arr);

QuickSort(arr, 0, arr.Length - 1);

Console.WriteLine("Arreglo ordenado:");
PrintArray(arr);

static void QuickSort(int[] arr, int low, int high)
{
    if (low < high)
    {
        int pivotIndex = Partition(arr, low, high);

        QuickSort(arr, low, pivotIndex - 1);
        QuickSort(arr, pivotIndex + 1, high);
    }
}

static int Partition(int[] arr, int low, int high)
{
    int pivot = arr[high];
    int i = low - 1;
    for (int j = low; j < high; j++)
    {
        if (arr[j] <= pivot)
        {
            i++;

            int temp = arr[i];
            arr[i] = arr[j];
            arr[j] = temp;
        }
    }

    int temp2 = arr[i + 1];
    arr[i + 1] = arr[high];
    arr[high] = temp2;

    return i + 1;
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

> En este ejemplo, el método `QuickSort` recibe un arreglo de enteros y los ordena utilizando el algoritmo de ordenamiento rápido. Después de ordenar el arreglo, se imprime en pantalla tanto el arreglo desordenado como el arreglo ordenado.
>