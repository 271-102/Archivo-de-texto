# Archivo-de-texto
casandra muyolema 
# Escritura de Archivo de Texto

# Abre (o crea si no existe) el archivo 'my_notes.txt' en modo escritura ('w')
with open("my_notes.txt", "w") as file:
    # Escribe tres líneas de notas personales
    file.write("1. Estudiar para el examen de matemáticas.\n")
    file.write("2. Llamar a Juan para coordinar el proyecto.\n")
    file.write("3. Leer el capítulo 4 del libro de historia.\n")

# Lectura de Archivo de Texto

# Abre el archivo 'my_notes.txt' en modo lectura ('r')
with open("my_notes.txt", "r") as file:
    # Lee cada línea del archivo utilizando readline() en un bucle
    print("Contenido del archivo my_notes.txt:")
    while True:
        linea = file.readline()
        if not linea:  # Si no hay más líneas, salir del bucle
            break
        print(linea.strip())  # strip() elimina los saltos de línea al final

# Nota: El uso de 'with' se encarga automáticamente de cerrar el archivo,
# por lo que no es necesario usar file.close()
