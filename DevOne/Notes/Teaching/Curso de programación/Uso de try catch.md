El `try` y `catch` son bloques de control de excepciones en C# que se utilizan para manejar errores en tiempo de ejecución. El bloque `try` contiene el código que puede generar una excepción, y el bloque `catch` atrapa la excepción y proporciona una manera de manejarla.

Aquí hay un ejemplo de código que divide dos números y maneja la excepción de división por cero:

```csharp
try
{
    Console.WriteLine("Introduce el primer número:");
    int num1 = int.Parse(Console.ReadLine());
    Console.WriteLine("Introduce el segundo número:");
    int num2 = int.Parse(Console.ReadLine());
    int result = num1 / num2;
    Console.WriteLine("El resultado de la división es: " + result);
}
catch (DivideByZeroException ex)
{
    Console.WriteLine("No se puede dividir por cero.");
}
catch (FormatException ex)
{
    Console.WriteLine("El formato del número es inválido.");
}
catch (Exception ex)
{
    Console.WriteLine("Se ha producido un error inesperado.");
}
finally
{
    Console.WriteLine("El programa ha finalizado.");
}
```

> En este ejemplo, si el usuario introduce un formato de número inválido o intenta dividir por cero, se mostrará un mensaje de error. De lo contrario, se mostrará el resultado de la división. El bloque `finally` se ejecutará independientemente de si se produjo una excepción o no.
> 

Es importante tener en cuenta que los bloques `catch` deben estar en orden de especificidad, desde las excepciones más específicas hasta las más generales. De lo contrario, puede producirse un error en tiempo de ejecución.