# Passes_time
#Esse programa contabiliza o número de partidas de um jogador e o número de gols

jogador = {}
partidas = []
jogador["Nome"] = str(input("Nome do jogador: "))
tot = int(input(f"Quantas partidas o {jogador['Nome']} jogou?: "))
for c in range(0,tot):
 partidas.append(int(input(f"Quantos gols na partida {c+1}: ")))
jogador["gols"] = partidas[:]
jogador["total"] = sum(partidas)
print("°°"*21)
print(jogador)
print("••"*21)
for k ,v in jogador.items():
 print(f"O campo {k} no valor de {v}")
print("__"*21)
print(f"O jogador {jogador['Nome']} jogou {jogador['gols']} na partida")
for i, v in enumerate(jogador["gols"]):
 print(f"Na partida {i+1} fez {v} gols")
print("\033[1;36m<<<FIM DO PROGRAMA>>>>\033[m")
print("\033[1;43m===VOLTE SEMPRE====\033[m")
