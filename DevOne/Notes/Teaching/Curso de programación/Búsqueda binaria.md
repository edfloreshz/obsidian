La búsqueda binaria es un algoritmo de búsqueda más eficiente que la búsqueda secuencial. Funciona dividiendo el arreglo en dos partes en cada iteración, hasta que el elemento buscado se encuentra o se determina que no está en el arreglo. Para utilizar la búsqueda binaria, es necesario que el arreglo esté ordenado.

Aquí hay un ejemplo de código de búsqueda binaria en C#:

```csharp
using System;

int[] arr = { 1, 2, 5, 5, 6, 9 };
Console.WriteLine("Arreglo: ");
PrintArray(arr);

Console.WriteLine("Ingrese un número a buscar: ");
int number = int.Parse(Console.ReadLine());

int index = BinarySearch(arr, number);
if (index == -1)
{
    Console.WriteLine("El número no se encuentra en el arreglo.");
}
else
{
    Console.WriteLine("El número se encuentra en el índice " + index + " del arreglo.");
}

static int BinarySearch(int[] arr, int number)
{
    int left = 0;
    int right = arr.Length - 1;
    while (left <= right)
    {
        int middle = (left + right) / 2;
        if (arr[middle] == number)
        {
            return middle;
        }
        else if (arr[middle] < number)
        {
            left = middle + 1;
        }
        else
        {
            right = middle - 1;
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

> En este ejemplo, el método `BinarySearch` recibe un arreglo de enteros ordenados y un número, y devuelve el índice del número en el arreglo si se encuentra, o un valor indicando que el número no está presente en el arreglo. Después de buscar el número, se imprime en pantalla el resultado de la búsqueda.
>