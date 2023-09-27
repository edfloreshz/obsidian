La programación orientada a objetos es un paradigma de programación que se basa en el uso de objetos y clases para modelar la realidad y resolver problemas. Aquí hay algunos de los principios fundamentales de la programación orientada a objetos.

## Abstracción

Se refiere a la capacidad de representar la esencia de un objeto sin tener en cuenta todos sus detalles. Por ejemplo, puede crear una clase `Vehículo` que tenga atributos comunes a todos los vehículos, como marca, modelo, año, etc., sin especificar exactamente qué tipo de vehículo es.

```csharp
public class Vehiculo
{
    public string Marca { get; set; }
    public string Modelo { get; set; }
    public int Año { get; set; }

    public Vehiculo(string marca, string modelo, int año)
    {
        Marca = marca;
        Modelo = modelo;
        Año = año;
    }
}
```

## Encapsulamiento

Se refiere a la habilidad de ocultar los detalles de implementación de un objeto y exponer solo los aspectos relevantes al usuario. Por ejemplo, puede tener una clase `CuentaBancaria` que tenga un método para retirar dinero, pero oculte la lógica detrás de la actualización del saldo.

```csharp
public class CuentaBancaria
{
    private decimal saldo;

    public decimal RetirarDinero(decimal cantidad)
    {
        if (saldo >= cantidad)
        {
            saldo -= cantidad;
            return cantidad;
        }
        else
        {
            return 0;
        }
    }
}
```

## Herencia

Se refiere a la capacidad de crear una nueva clase a partir de una clase existente, heredando sus atributos y métodos. Por ejemplo, puede crear una clase `Automóvil` que herede de la clase `Vehículo` y agregue atributos y métodos específicos de un automóvil.

```csharp
public class Automovil : Vehiculo
{
    public int Puertas { get; set; }

    public Automovil(string marca, string modelo, int año, int puertas)
        : base(marca, modelo, año)
    {
        Puertas = puertas;
    }
}
```

## Polimorfismo

Se refiere a la capacidad de un objeto para tomar múltiples formas. Por ejemplo, puede tener una lista de objetos `Vehículo` que contengan tanto automóviles como motocicletas, y llamar un método `MostrarInformacion` en cada clase que devuelva información sobre el objeto. Luego, puede recorrer la lista y llamar a ese método para cada objeto, y cada objeto devolverá su información específica:

```csharp
public class Vehiculo
{
    public string Marca { get; set; }
    public string Modelo { get; set; }
    public int Año { get; set; }

    public Vehiculo(string marca, string modelo, int año)
    {
        Marca = marca;
        Modelo = modelo;
        Año = año;
    }

    public virtual string MostrarInformacion()
    {
        return $"Marca: {Marca}, Modelo: {Modelo}, Año: {Año}";
    }
}

public class Automovil : Vehiculo
{
    public int Puertas { get; set; }

    public Automovil(string marca, string modelo, int año, int puertas)
        : base(marca, modelo, año)
    {
        Puertas = puertas;
    }

    public override string MostrarInformacion()
    {
        return $"{base.MostrarInformacion()}, Puertas: {Puertas}";
    }
}

public class Motocicleta : Vehiculo
{
    public int Cilindrada { get; set; }

    public Motocicleta(string marca, string modelo, int año, int cilindrada)
        : base(marca, modelo, año)
    {
        Cilindrada = cilindrada;
    }

    public override string MostrarInformacion()
    {
        return $"{base.MostrarInformacion()}, Cilindrada: {Cilindrada}";
    }
}

List<Vehiculo> vehiculos = new List<Vehiculo>
{
    new Automovil("Toyota", "Camry", 2020, 4),
    new Motocicleta("Yamaha", "R1", 2020, 1000)
};

foreach (var vehiculo in vehiculos)
{
    Console.WriteLine(vehiculo.MostrarInformacion());
}
```

Estos son solo algunos ejemplos de los principios fundamentales de la programación orientada a objetos. Hay muchas otras características y conceptos que se pueden utilizar para crear aplicaciones poderosas y robustas.