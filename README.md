def sumar(a, b):
    return a + b

def restar(a, b):
    return a - b

def multiplicar(a, b):
    return a * b

def dividir(a, b):
    if b == 0:
        return "Error: División por cero no permitida."
    else:
        return a / b

def calcular():
    print("Calculadora")
    print("Operaciones disponibles: ")
    print("1. Sumar")
    print("2. Restar")
    print("3. Multiplicar")
    print("4. Dividir")
    
    # Solicitar al usuario que seleccione una operación
    operacion = input("Seleccione una operación (1/2/3/4): ")

    # Solicitar al usuario los dos números para la operación
    num1 = float(input("Ingrese el primer número: "))
    num2 = float(input("Ingrese el segundo número: "))

    # Realizar la operación seleccionada
    if operacion == "1":
        print(f"Resultado: {num1} + {num2} = {sumar(num1, num2)}")
    elif operacion == "2":
        print(f"Resultado: {num1} - {num2} = {restar(num1, num2)}")
    elif operacion == "3":
        print(f"Resultado: {num1} * {num2} = {multiplicar(num1, num2)}")
    elif operacion == "4":
        resultado_division = dividir(num1, num2)
        print(f"Resultado: {num1} / {num2} = {resultado_division}")
    else:
        print("Operación no válida. Por favor, seleccione una operación válida.")

# Ejecutar la calculadora
calcular()

