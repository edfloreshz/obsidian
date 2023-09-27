# Estructuras

Las estructuras en programación son como cajas pequeñas que contienen diferentes tipos de información. Piensa en ellas como una lista de compras que tienes en tu casa. La lista de compras contiene diferentes tipos de información, como el nombre de los productos que quieres comprar, la cantidad de cada producto, el precio, etc.

De manera similar, en la programación, puedes crear una estructura que represente un producto y contenga información sobre ese producto, como su nombre, precio, cantidad, etc. De esta manera, puedes usar esta estructura para almacenar y manipular información sobre un producto de manera organizada y estructurada.

```csharp
struct Producto
{
    public string Nombre;
    public decimal Precio;
    public int Cantidad;

    public decimal TotalPrice()
    {
        return Precio * Cantidad;
    }
}
```

Aquí hay un ejemplo de código que usa la estructura `Producto`:

```csharp
Producto producto;
producto.Nombre = "Manzana";
producto.Precio = 10;
producto.Cantidad = 5;

Console.WriteLine("Nombre del producto: " + producto.Nombre);
Console.WriteLine("Precio total: " + producto.TotalPrice());
```

> En este ejemplo, estamos creando una variable `product1` de tipo `Product` y asignándole valores a sus campos. Luego, estamos imprimiendo el nombre y el precio total del producto en la consola.
> 

Las estructuras se declaran de manera similar a las clases, pero tienen algunas diferencias clave. Por ejemplo, las estructuras son tipos de valor, lo que significa que cada vez que se pasa una estructura a una función o se asigna a una variable, se hace una copia de la estructura en lugar de pasar una referencia a la misma estructura. Esto significa que las estructuras son adecuadas para representar objetos simples o pequeños, mientras que las clases son adecuadas para representar objetos más complejos.