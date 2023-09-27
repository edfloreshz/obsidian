Los "**identificadores**" o "**símbolos**" son los nombres que se proporcionan para variables, tipos, funciones y etiquetas del programa.

Los nombres de identificadores deben diferir en ortografía, mayúsculas y minúsculas de cualquier palabra clave.

No se puede utilizar palabras clave como identificadores; se **reservan** para uso especial.

## Ejemplo

```csharp
// Uso correcto de identificadores
var nombreDeLaVariable; 

// Uso incorrecto de identificadores, no se puede hacer uso de una palabra reservada como identificador.
var var; 
```

## **Convención de nombres**

Es un conjunto de reglas para la elección de la secuencia de caracteres que se utilice para los identificadores que denoten variables, tipos, funciones y otras entidades en el código fuente y la documentación.

### camelCase

Comienzas un nombre con una letra minúscula. Si el nombre tiene varias palabras, las palabras posteriores comenzarán con una letra mayúscula, sin espacios.

```csharp
var nombreDeLaVariable; 
```

### snake_case

Todas las palabras comenzarán con letras minúsculas y usará un guión bajo `_` para separar las palabras.

```csharp
var nombre_de_la_variable; 
```

### kebab-case

El `kebab-case` es similar al `snake_case`, pero usa un guión `-` en lugar de un guión bajo `_` para separar las palabras.

```csharp
var nombre-de-la-variable; 
```

### PascalCase

A diferencia de los ejemplos anteriores, los nombres en `PascalCase` comienzan con una letra mayúscula. En el caso de los nombres con varias palabras, todas las palabras comenzarán con letras mayúsculas.

```csharp
var NombreDeLaVariable;
```

El tipo de convencion de nombres a utilizar lo definira el lenguaje que se utilice.