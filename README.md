print("****************************************************")
print("*Programa para cambiar mensajes de letras a numeros*")
print("****************************************************\n")

def letra_a_numero(letra):
    letra = letra.upper()
    if 'A' <= letra <= 'Z':
        return str(ord(letra) - ord('A') + 1)
    else:
        return letra  # Conservar caracteres que no son letras

mensaje = input("Ingresa un mensaje: ")
mensaje = '-'.join([letra_a_numero(letra) for letra in mensaje])

print(f"Mensaje en números: {mensaje}")
