Las declaraciones `if` también se pueden anidar para permitir un mayor control sobre el flujo de un programa. Esto significa que una declaración `if` puede contener una o más declaraciones `if` adicionales dentro de ella.

Aquí hay un ejemplo en C#:

```csharp
using System;

namespace NestedIfExample
{
    class Program
    {
        static void Main(string[] args)
        {
            int number = 5;

            if (number > 0)
            {
                Console.WriteLine("El número es positivo");

                if (number % 2 == 0)
                {
                    Console.WriteLine("El número es par");
                }
                else
                {
                    Console.WriteLine("El número es impar");
                }
            }
            else
            {
                Console.WriteLine("El número es negativo");
            }
        }
    }
}
```

> En este ejemplo, la primera declaración `if` verifica si `number` es mayor que `0`. Si esta condición es verdadera, se ejecuta el código dentro de la primera declaración `if`, que a su vez contiene una segunda declaración `if` que verifica si `number` es par o impar. En función de esta segunda condición, se imprime en la consola "El número es par" o "El número es impar". Si la primera condición es falsa, se ejecuta el código dentro de la declaración `else` y se imprime en la consola "El número es negativo".
> 

Las declaraciones `if` anidadas permiten a los programadores realizar múltiples comprobaciones y tomar decisiones basadas en múltiples condiciones. Esto puede ser muy útil en aplicaciones complejas que requieren un control fino sobre el flujo de un programa.