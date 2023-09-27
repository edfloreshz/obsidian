# Interfaces como contratos

Las interfaces en programación son como contratos que definen un conjunto de reglas que deben ser seguidas por cualquier cosa que quiera usar esa interfaz. Son como promesas que hacen los objetos de programación de que pueden hacer ciertas cosas.

Por ejemplo, imagina que quieres dibujar un círculo en la pantalla. Para hacer esto, necesitas un objeto que sepa cómo dibujarse. Este objeto puede hacer una promesa de que sabe cómo dibujarse mediante la implementación de una interfaz llamada `IDrawable`. Esta interfaz puede decir que todos los objetos que la implementen deben tener un método llamado `Draw()` que dibuje el objeto en la pantalla.

Entonces, la clase `Circle` puede implementar esta interfaz y proporcionar su propia implementación para el método `Draw()`. De esta manera, sabemos que la clase `Circle` sabe cómo dibujarse porque cumple con las reglas definidas en la interfaz `IDrawable`.

```csharp
interface IDrawable
{
    void Draw();
}
```

> En este ejemplo, la interfaz `IDrawable` define un contrato para un objeto que puede ser dibujado. La interfaz define un solo método, `Draw()`, que debe ser implementado por cualquier clase o struct que implemente la interfaz.
> 

Las clases o structs que implementan una interfaz deben proporcionar implementaciones para todos los métodos y propiedades definidos en la interfaz. Por ejemplo:

```csharp
class Circle : IDrawable
{
    public void Draw()
    {
        Console.WriteLine("Drawing a Circle");
    }
}
```