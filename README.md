def podio_olimpico(tempo_chegada1,tempo_chegada2,tempo_chegada3):
  if (tempo_chegada1 < tempo_chegada2):
    if (tempo_chegada2 < tempo_chegada3):
      resultado = f"1 - {tempo_chegada1} minutos\n2 - {tempo_chegada2} minutos\n3 - {tempo_chegada3} minutos\n"
    else:
      if (tempo_chegada1 < tempo_chegada3):
        resultado = f"1 - {tempo_chegada1} minutos\n2 - {tempo_chegada3} minutos\n3 - {tempo_chegada2} minutos\n" 
      else:
        resultado = f"1 - {tempo_chegada3} minutos\n2 - {tempo_chegada1} minutos\n3 - {tempo_chegada2} minutos\n"
  else:
    if (tempo_chegada2 < tempo_chegada3):
      if (tempo_chegada1 < tempo_chegada3):
        resultado = f"1 - {tempo_chegada2} minutos\n2 - {tempo_chegada1} minutos\n3 - {tempo_chegada3} minutos\n"
      else:
        resultado = f"1 - {tempo_chegada2} minutos\n2 - {tempo_chegada3} minutos\n3 - {tempo_chegada1} minutos\n"
    else:
      resultado = f"1 - {tempo_chegada3} minutos\n2 - {tempo_chegada2} minutos\n3 - {tempo_chegada1} minutos\n"
  return resultado

tempo_chegada1 = int(input("insira o tempo de chegada do 1 competidor, em minutos"))
tempo_chegada2 = int(input("insira o tempo de chegada do 2 competidor, em minutos"))
tempo_chegada3 = int(input("insira o tempo de chegada do 3 competidor, em minutos"))

resultado = podio_olimpico(tempo_chegada1,tempo_chegada2,tempo_chegada3)
print(resultado)
