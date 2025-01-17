# Numeros
Es un juego que consiste en adivinar el numero
import random  # Importamos el módulo para generar números aleatorios

# Generamos un número aleatorio entre 1 y 100
numero_secreto = random.randint(1, 100)

print("¡Bienvenido al juego de Adivina el Número!")
print("Estoy pensando en un número entre 1 y 100. ¿Puedes adivinar cuál es?")

# Variable para controlar si el usuario adivinó
adivinado = False

# Ciclo para seguir preguntando hasta que el usuario adivine
while not adivinado:
    # Pedimos al usuario que ingrese su adivinanza
    intento = int(input("Escribe tu número: "))
    
    # Verificamos si es correcto
    if intento == numero_secreto:
        print("¡Felicidades! Adivinaste el número secreto.")
        adivinado = True
    elif intento < numero_secreto:
        print("El número es más grande. ¡Inténtalo de nuevo!")
    else:
        print("El número es más pequeño. ¡Sigue intentando!")

print("Gracias por jugar. ¡Hasta la próxima!")
