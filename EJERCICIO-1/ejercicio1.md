# Merca Excel

El excel es una de las herramientas más usada en Mercadona y nos da una serie de funciones interesantes como: COUNTIF, SUMIF y AVERAGEIF.

## Criterios
- La firma de los métodos admitirá 2 parámetros:
    - El primero de ellos debe de ser un array de `valores` (puede ser cualquier tipo de dato).
    - El `criterio`, que puede recibir cualquier tipo de dato (String, Integer o Float).
        - Que se reciba un integer o un float indica igualdad.
        - Un String puede indicar >, >=, <, <= o <> para poder comparar con un integer. En la función `COUNT_IF` con un String sin el operador, indica igualdad.

## Ejemplos
```
count_if([1,3,5,7,9], 3)
1

count_if(["John","Steve","John"], "John")
2

sum_if([2,4,6,-1,3,1.5],">0")
16.5

average_if([99,95.5,0,83],"<>0")
92.5
```

