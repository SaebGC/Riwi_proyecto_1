# Calculadora en Python

Este programa es una calculadora de consola que permite realizar operaciones matemáticas básicas.

## Operaciones disponibles

- Suma
- Resta
- Multiplicación
- División
- Potencia
- Raíz cuadrada
- Porcentaje
- Módulo
- Promedio

## Código

```python
while True:
    print("1. Suma")
    print("2. Resta")
    print("3. Multiplicación")
    print("4. División")
    print("5. Potencia")
    print("6. Raíz cuadrada")
    print("7. Porcentaje")
    print("8. Modulo")
    print("9. Promedio")
    print("10. Salir")   

    opcion = int(input("Seleccione una opción(1-10): "))

    if opcion == 10:
        print("Acabas de salir.")
        break

    elif opcion == 1:
        num1 = int(input("Ingrese el primer número: "))
        num2 = int(input("Ingrese el segundo número: "))
        resultado = num1 + num2
        print(f"El resultado de la suma es: {resultado}")

    elif opcion == 2:
        num1 = int(input("Ingrese el primer número: "))
        num2 = int(input("Ingrese el segundo número: "))
        resultado = num1 - num2
        print(f"El resultado de la resta es: {resultado}")

    elif opcion == 3:
        num1 = int(input("Ingrese el primer número: "))
        num2 = int(input("Ingrese el segundo número: "))
        resultado = num1 * num2
        print(f"El resultado de la multiplicación es: {resultado}")
    
    elif opcion == 4:
        num1 = int(input("Ingrese el primer número: "))
        num2 = int(input("Ingrese el segundo número: "))
        if num2 != 0:
            resultado = num1 / num2
            print(f"El resultado de la división es: {resultado}")
        else:
            print("Error: No se puede dividir por cero.")
    
    elif opcion == 5:
        num1 = int(input("Ingrese la base: "))
        num2 = int(input("Ingrese el exponente: "))
        resultado = num1 ** num2
        print(f"El resultado de la potencia es: {resultado}")

    elif opcion == 6:
        num = int(input("Ingrese el número: "))
        if num >= 0:
            resultado = num ** 0.5
            print(f"El resultado de la raíz cuadrada es: {resultado}")
        else:
            print("Error: No se puede calcular la raíz cuadrada de un número negativo.")

    elif opcion == 7:
        num1 = int(input("Ingrese el número: "))
        num2 = int(input("Ingrese el porcentaje: "))
        resultado = (num1 * num2) / 100
        print(f"El resultado del porcentaje es: {resultado}")

    elif opcion == 8:
        num1 = int(input("Ingrese el primer número: "))
        num2 = int(input("Ingrese el segundo número: "))
        if num2 != 0:
            resultado = num1 % num2
            print(f"El resultado del modulo es: {resultado}")
        else:
            print("Error: No se puede calcular el modulo por cero.")

    elif opcion == 9:
        cantidad = int(input("¿Cuántos números desea promediar? "))
        suma = 0
        for i in range(cantidad):
            num = int(input(f"Ingrese el número {i+1}: "))
            suma += num
        resultado = suma / cantidad
        print(f"El resultado del promedio es: {resultado}")
```

## Notas importantes

> **División y Módulo:** El programa valida que el divisor no sea cero antes de operar.

> **Raíz cuadrada:** Solo acepta números positivos o cero.

> **Salir:** Selecciona la opción `10` para cerrar el programa.
