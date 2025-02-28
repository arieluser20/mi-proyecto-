# mi-proyecto-
 Repositorio para el desarrollo de mi proyecto académico.
git clone URL_DEL_REPOSITORIO
if condición:
    # Bloque de código si la condición es verdadera
else:
    # Bloque de código si la condición es falsa
    # Definir la matriz 3x3
matriz = [
    [5, 8, 3],
    [4, 1, 9],
    [7, 2, 6]
]

def buscar_valor(matriz, valor):
    for i in range(len(matriz)):
        for j in range(len(matriz[i])):
            if matriz[i][j] == valor:
                return (i, j)  # Devuelve la posición si se encuentra el valor
    return None  # Devuelve None si no se encuentra el valor

# Valor a buscar
valor_buscado = int(input("Ingrese el valor a buscar en la matriz: "))

# Buscar el valor en la matriz
resultado = buscar_valor(matriz, valor_buscado)

# Mostrar el resultado
if resultado:
    print(f"El valor {valor_buscado} se encontró en la posición {resultado}.")
else:
    print(f"El valor {valor_buscado} no se encontró en la matriz.")

# Definir la matriz 3x3
matriz = [
    [5, 8, 3],
    [4, 1, 9],
    [7, 2, 6]
]

def bubble_sort(fila):
    n = len(fila)
    for i in range(n):
        for j in range(0, n - i - 1):
            if fila[j] > fila[j + 1]:
                fila[j], fila[j + 1] = fila[j + 1], fila[j]  # Intercambio de valores
    return fila

# Mostrar matriz original
print("Matriz original:")
for fila in matriz:
    print(fila)

# Fila a ordenar (por ejemplo, la segunda fila -> índice 1)
fila_a_ordenar = 1
matriz[fila_a_ordenar] = bubble_sort(matriz[fila_a_ordenar])

# Mostrar matriz con la fila ordenada
print("\nMatriz con la fila ordenada:")
for fila in matriz:
    print(fila)

