# Autor
Juan Andrés Pico 
# Completando libreria 
- Adición de vectores complejos.
- Inverso (aditivo) de un vector complejo.
- Multiplicación de un escalar por un vector complejo.
- Adición de matrices complejas.
- Inversa (aditiva) de una matriz compleja.
- Multiplicación de un escalar por una matriz compleja.
- Transpuesta de una matriz/vector
- Conjugada de una matriz/vector
- Adjunta (daga) de una matriz/vector
- Producto de dos matrices (de tamaños compatibles)
- Función para calcular la "acción" de una matriz sobre un vector.
- Producto interno de dos vectores
- Norma de un vector
- Distancia entre dos vectores
- Revisar si una matriz es unitaria
- Revisar si una matriz es Hermitiana
- Producto tensor de dos matrices/vectores

# Ejecución del programa
Para un correcto uso del programa se tiene una funcion main que invoca las demás funciones que se mostraron enumeradas arriba, para el correcto uso usted puede cambiar los valores de `lista1`, `lista2`, `lista3`
![](/img/main.png)
Tambien se recomienda que para no leer tantos valores en consola se documente las funciones ya revisadas para no tener ningun mal entendido 
![](/img/revisando%20consola.png)

Como se puede ver muestra todo el proceso por el que tiene que pasar para la suma de vectores usando la anterior libreria ya creada.
Para al final tener el resultado puesto a calculado.

## Ejemplos 
Ejemplo # 1 . Se desea buscar la suma de matrices complejas y para su implementación se creo este codigo 
```python
def sumaMatricesComplejas(mat1, mat2):
    for i in range(len(mat1)):
        for j in range(len(mat1[0])):
            mat1[i][j] = sumarComplejos(mat1[i][j], mat2[i][j])
    print("suma de matrices complejas : " + str(mat1))
    return mat1
```

La cual como se menciono anteriormente reutiliza la calculadora con la funcion sumarComplejos. viendolo más graficamente podemos probarlo con los valores 
![](/img/sumadematrices.png)

Dando como resultado el anteriormente visto 
![](/img/revisando%20consola.png)