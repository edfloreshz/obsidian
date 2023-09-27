Los caracteres son representaciones de letras o símbolos alfabéticos. 

## Declaración

Para declarar una variable de tipo `char` se debe asignar una letra o símbolo rodeado de comillas simples. `''`

```csharp
char a = 'A';
char b = 'B';

string ab = a + b; // "AB"
```

Los caracteres se representan de diferentes maneras.

## ASCII

[Tabla de caracteres](http://www.csc.villanova.edu/~tway/resources/ascii-table.html)

El ASCII es, básicamente, un código de caracteres que tiene su base en el alfabeto romano o latino. Esto quiere decir que el ASCII sirve para convertir, a través de una serie de reglas, un carácter que forma parte de un lenguaje natural (como una letra de un alfabeto) en un símbolo que pertenece a otra clase de sistema representativo.

Aunque no es la única manera, una de las representaciones mas utilizadas es `UTF-8`, dado a su flexibilidad y capacidad para mostrar mas caracteres que `ASCII`.

## UTF-8

[Tabla de caracteres](https://www.ssec.wisc.edu/~tomw/java/unicode.html)

UTF-8 es un formato de codificación de caracteres `Unicode` que ha revolucionado el mundo digital. Es el responsable de que tu navegador o tu cliente de correo te muestre el contenido del texto correctamente decodificado, sin errores ni caracteres extraños.

### Tipos de codificación

Unicode define cada carácter o símbolo mediante un nombre e identificador numérico, el llamado punto de código. Cuando se ha asignado un código a un carácter, se dice que dicho carácter está codificado.

Para que ese número o código sea entendido por el ordenador debe estar codificado. Las formas de codificación de Unicode reglamentan la forma en que los puntos de código se transformarán en unidades inteligibles por una máquina. Existen tres formas de codificación bajo el nombre UTF (Unicode Transformation Format):

- UTF-8: codificación orientada a byte con símbolos de longitud variable.
- UTF-16: codificación de 16 bits de longitud variable optimizada para la representación del plano básico multilingüe (BMP).
- UTF-32: codificación de 32 bits de longitud fija, y la más sencilla de las tres.

## Unicode

Las computadoras trabajan con un método para representar los caracteres que se muestran en una pagina web o en el servicio de correo que utilizamos a diario. Ese método se denomina `Unicode` y funciona a través de números.

Unicode cubre todos los caracteres de todos los sistemas de escritura del mundo, modernos y antiguos. También incluye símbolos técnicos, signos de puntuación y muchos otros caracteres que se usan para escribir texto. Esto le permite satisfacer las necesidades de todo tipo de usuarios, ya 
sea en el mundo empresarial o académico.

Unicode también es capaz de representar emojis.

![Untitled](Notes/Teaching/Curso%20de%20programación/Caracteres/Untitled.png)