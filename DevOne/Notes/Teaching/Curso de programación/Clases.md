# Clases

Las clases son una característica fundamental de la programación orientada a objetos y se utilizan para modelar objetos reales en el código.

## Definición de clases

Una clase es una estructura que define un conjunto de atributos (datos) y métodos (acciones) que describen un objeto. Por ejemplo, si queremos modelar un auto, podemos crear una clase `Car` que tenga atributos como el modelo, la marca, el color, etc. y métodos como encender el motor, acelerar, frenar, etc.

Aquí hay un ejemplo de una clase en C# que representa un producto:

```csharp
class Product
{
    public string Name { get; set; }
    public decimal Price { get; set; }
    public int Quantity { get; set; }

    public decimal TotalPrice()
    {
        return Price * Quantity;
    }
}
```

## Instancias de clases

Una vez que se define una clase, se pueden crear objetos o "instancias" de ella. Cada instancia tendrá sus propios valores para los atributos y podrá ejecutar los métodos de la clase. Por ejemplo, podemos crear dos objetos `Car`: uno para un Ford Mustang y otro para un Toyota Camry.

Aquí hay un ejemplo de cómo crear una instancia de la clase `Product`:

```csharp
Product product1 = new Product();
product1.Name = "Product 1";
product1.Price = 10;
product1.Quantity = 5;
```

## Constructores

Los constructores son métodos especiales que se utilizan para inicializar una nueva instancia de una clase. Al crear una instancia de una clase, se invoca automáticamente su constructor. Por ejemplo, podemos crear un constructor en la clase `Car` que asigne valores iniciales a los atributos cuando se crea una nueva instancia.

```csharp
class Product
{
    public string Name { get; set; }
    public decimal Price { get; set; }
    public int Quantity { get; set; }

    public Product(string name, decimal price, int quantity)
    {
        Name = name;
        Price = price;
        Quantity = quantity;
    }

    public decimal TotalPrice()
    {
        return Price * Quantity;
    }
}
```

## Destructores

Los destructores son métodos especiales que se invocan automáticamente cuando un objeto se elimina. Los destructores se utilizan para liberar recursos asociados con un objeto antes de que se destruya.

```csharp
class Product
{
    public string Name { get; set; }
    public decimal Price { get; set; }
    public int Quantity { get; set; }

    ~Product()
    {
        // Código para liberar recursos aquí
    }

    public decimal TotalPrice()
    {
        return Price * Quantity;
    }
}
```

## Sobrecarga de constructores

La sobrecarga de constructores es una técnica que permite tener varios constructores con diferentes argumentos en una misma clase. Esto se hace para que sea más fácil crear objetos con diferentes conjuntos de valores iniciales.

```csharp
class Product
{
    public string Name { get; set; }
    public decimal Price { get; set; }
    public int Quantity { get; set; }

    // Constructor sin argumentos
    public Product()
    {
        Name = "Product";
        Price = 0;
        Quantity = 0;
    }

    // Constructor con argumentos
    public Product(string name, decimal price, int quantity)
    {
        Name = name;
        Price = price;
        Quantity = quantity;
    }

    public decimal TotalPrice()
    {
        return Price * Quantity;
    }
}
```

## Propiedades

Las propiedades en programación son una forma de acceder y modificar valores de una clase de manera controlada. Se comportan como atributos, pero proporcionan un mayor nivel de control y seguridad, ya que se pueden establecer reglas y validaciones para el acceso y la asignación de valores.

El acceso a los valores de una propiedad se hace mediante la sintaxis de una variable, pero el código real detrás de una propiedad puede realizar cualquier tarea que se requiera, como validar un valor o calcular un valor basado en otras propiedades de la clase.

Este es un ejemplo de código en C# para una clase con una propiedad llamada `Name`:

```csharp
class Person
{
    private string name;

    public string Name
    {
        get
        {
            return name;
        }
        set
        {
            if (!string.IsNullOrEmpty(value))
            {
                name = value;
            }
        }
    }
}
```

En este ejemplo, la propiedad `Name` tiene una implementación `get` y una implementación `set`, lo que significa que se puede acceder y asignar un valor a la propiedad. La implementación `get` devuelve el valor de la variable privada "name", mientras que la implementación `set` realiza una validación para asegurarse de que el valor que se está asignando sea válido antes de asignarlo a la variable `name`.