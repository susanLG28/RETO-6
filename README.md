# RETO-6
### 1. Imprimir un listado con los números del 1 al 100 cada uno con su respectivo cuadrado.
    for i in range(1, 101):
        print(f"el cuadrado de {i} es {i**1}")

### 2. Imprimir un listado con los números impares desde 1 hasta 999 y seguidamente otro listado con los números pares desde 2 hasta 1000.
    print("numeros impares del 1 al 999")
    for i in range(1, 1000, 2):
        print(f"{i}")
    print("numeros impares del 2 al 1000")
    for i in range(2, 1001, 2):
        print(f"{i}")

### 3. Imprimir los números pares en forma descendente hasta 2 que son menores o iguales a un número natural n ≥ 2 dado
    n = int(input("ingrese un numero: "))
    if n >= 2:
        print("los numeros pares son:")
        for i in range(n, 0, -1):
            if i % 2 == 0:
                print(f"{i}")
    else:
        print("el numero debe ser mayor o igual a 2")
### 4. Imprimir el factorial de un número natural n dado.
    n = int(input("ingrese el numero entero positivo: "))
    factorial = 1
    for i in range(1, n + 1):
        factorial *= i
    print(f"el factorial de {n} es {factorial}")
### 5. Implementar un programa que ingrese un número de 2 a 50 y muestre sus divisores.
    n = int(input("ingrese un numero entre 2 y 50: "))
    print(f"los divisores de {n} son:")
    for i in range(n, 0, -1):
        if n % i == 0:
            print(i)
### 6. Implementar el algoritmo que muestre los números primos del 1 al 100.
    def numero_primo(n):
        if n < 2:
            return False
        for i in range(2, int(n**0.5) +1):
            if n % i == 0:
                return False
        return True

    print("numeros primos del 1 al 100")
    for i in range(1, 101):
        if numero_primo(i):
            print(i)

