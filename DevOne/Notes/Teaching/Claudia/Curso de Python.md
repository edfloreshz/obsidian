# Tipos de datos

### Numericos

 - Numeros enteros: negativos, positivos y 0. (Int)

                                 5, 36, 0, -12

 - Numeros en coma flotante: tienen decimales. Positivos, negativos, 0.0. (Float)

                                                 8.9, 0.0, -367.9

### Booleanos:

Representa los valores de verdad, importantes en expresiones condicionales y ciclos.

 - True

 - False

### Cadenas de caracteres (String)

Secuencia de caracteres encerrados entre comillas usados para representar texto en el programa. (str)

“Python” o ‘Python’

**Caracteristicas:**

Length (len): numero de caracteres que posee.

```python
nombre = nora
len (nombre)
4
```

**Indexacion:**

Empezando por el 0…

```python
palabra = "python"
Palabra [0]
'p'
palabra [1]
'y'
```

**Rebanado (slicing):**

Obtener una porcion de una cadena de caracteres.

```python
palabra = "python"
palabra[1:4]
'yth'
```

Saltar un caracter al siguiente: <cadena>[inicio:fin:paso]

```python
palabra = "python"
palabra[1:6:2]
'yhn'
```