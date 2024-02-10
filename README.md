# Actividad3
Tarea
def D (diccionario):

  nombre = input("Nombre deseado: ")

  elemento = input("Ingrese el elemento: ")

  diccionario[nombre] = elemento

  print("Elemento agregado ")



def Buscar (diccionario):

  nombre = input("Buscador: ")

  if nombre in diccionario:

    print("Descripción:", diccionario[nombre])

  else:

    print("no existe")



def cambiar (diccionario):

  nombre = input("cambiar: ")

  if nombre in diccionario:

    elemento = input("elemento: ")

    diccionario[nombre] = elemento

    print("Elemento cambiado")

  else:

    print("El elemento no se encuentra en el diccionario.")



def borrar(diccionario):

  nombre = input(" borrar: ")

  if nombre in diccionario:

    del diccionario[nombre]

    print("Elemento borrado ")

  else:

    print("No esta")



def mostrar (diccionario):

  print("Contenido:")

  for nombre, elemento in diccionario.items():

    print("{nombre}: {elemento}")



  while True:

    print("Menú:")

    print("1-Agregar un elemento")

    print("2-Buscar un elemento")

    print("3-Cambiar un elemento ")

    print("4-Borrar un elemento ")

    print("5-Mostrar el diccionario")

    print("6-Salir")



    opcion = input("Seleccione una opción: ")



    if opcion == "1":

      agregar(diccionario)

    elif opcion == "2":

      buscar(diccionario)

    elif opcion == "3":

      cambiar(diccionario)

    elif opcion == "4":

      borrar(diccionario)

    elif opcion == "5":

      mostrar(diccionario)

    elif opcion == "6":

      print("BYE")
