# Constantes

Las constantes incrementa la claridad y facilita el mantenimiento de programas, tiene escencialmente el mismo uso que una variable, con una diferencia clave, las constantes ******************no pueden cambiar******************.

La mayoria de los lenguajes utilizan la palabra clave `const` para declarar una constante.

```csharp
const VERSION = "1.0.0";
```

## Ejemplo

Imaginemos que tenemos un programa y queremos mostrar la version con diferentes formatos.

```csharp
var versionConPrefijo = "V1.0.0";
var versionConEtiqueta = "Version 1.0.0";
```

Esto puede provovar problemas, cada vez que necesitemos modificar el numero de la version, habria que modificar cada valor que contenga el numero, esto puede volverse tedioso y es propenso a errores.

Un uso efectivo de constantes seria el siguiente:

```csharp
const VERSION = "1.0.1";

var versionConPrefijoV = "V" + VERSION;
var versionConPuntoAlFinal = "Version " + VERSION;
```

Dado a que definimos la constante con el numero de version, cada vez que queramos cambiar la version, solo sera necesario modificar esa constante y todos los lugares donde se utiliza se actualizaran automaticamente tambien.