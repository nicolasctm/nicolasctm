puntajes=[]
tipos_de_jugadores=[]

def Registrar_puntajes_torneo():
    while True:
          id_jugador = input("ingrese su id: ")
          nombre = input("ingrese su nombre: ")
          apellido = input("ingrese su apellido: ")
          juego = input("ingrese juego: ")
          if juego == "fornite":
                while True:
                    try:
                        puntaje = int(input("ingrese puntos: "))
                        puntajes.append(puntaje)
                        break
                    except:
                         print("ingrese solo digitos")  
                tipo_de_jugador= input("principiante - avanzado - experto): ")
                if tipo_de_jugador == "principiante":
                    tipos_de_jugadores.append(tipo_de_jugador)
                    print("datos registrados")
                    break
                elif tipo_de_jugador == "avanzado":
                    tipos_de_jugadores.append(tipo_de_jugador)
                    print("datos registrdos")
                    break
                elif tipo_de_jugador == "experto":
                     tipos_de_jugadores.append(tipos_de_jugadores)
                     print("datos registrados")
                     break
                else:
                     print("este tipo de jugador no existe")
          elif juego == "valorant":
                while True:
                    try:
                        puntaje = int(input("ingrese puntos: "))
                        puntajes.append(puntaje)
                        break
                    except:
                         print("ingrese solo digitos")  
                tipo_de_jugador= input("principiante - avanzado - experto): ")
                if tipo_de_jugador == "principiante":
                    tipos_de_jugadores.append(tipo_de_jugador)
                    print("datos registrados")
                    break
                elif tipo_de_jugador == "avanzado":
                    tipos_de_jugadores.append(tipo_de_jugador)
                    print("datos registrdos")
                    break
                elif tipo_de_jugador == "experto":
                     tipos_de_jugadores.append(tipos_de_jugadores)
                     print("datos registrados")
                     break
                else:
                     print("este tipo de jugador no existe")
            
          elif juego == "fifa":
                while True:
                    try:
                        puntaje = int(input("ingrese puntos: "))
                        puntajes.append(puntaje)
                        break
                    except:
                         print("ingrese solo digitos")  
                tipo_de_jugador= input("principiante - avanzado - experto): ")
                if tipo_de_jugador == "principiante":
                    tipos_de_jugadores.append(tipo_de_jugador)
                    print("datos registrados")
                    break
                elif tipo_de_jugador == "avanzado":
                    tipos_de_jugadores.append(tipo_de_jugador)
                    print("datos registrdos")
                    break
                elif tipo_de_jugador == "experto":
                     tipos_de_jugadores.append(tipos_de_jugadores)
                     print("datos registrados")
                     break
                else:
                     print("este tipo de jugador no existe")
          else:
            print("juego no encontrado")
            return      
                
            
def Listar_puntajes():
     print(puntajes)

def Imprimir_tipo():
     print(tipos_de_jugadores)
    
          

def menu():
    while True:
        print("---menu---")
        print("1-Registrar puntajes torneo")
        print("2-Listar los todos puntajes")
        print("3-Imprimir por Tipo")
        print("4-Salir del programa")

        opcion = input("Igrese Opcion: ")
        
        if opcion == "1":
                Registrar_puntajes_torneo()
        elif opcion =="2":
                Listar_puntajes()
        elif opcion =="3":
                Imprimir_tipo()
        elif opcion =="4":
            print("Haz salido del programa con exito")  
            break         
        else:
            print("opcion invalida")
            return menu()


menu()
