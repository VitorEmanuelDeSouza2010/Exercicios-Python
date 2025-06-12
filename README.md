# Exercicios-Python
#Apenas alguns exercicios em Python feitos durante a aula do curso.

#1)>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
n1 = input("Digite o 1º número: ")
n2 = input("Digite o 2º número: ")
n3 = input("Digite o 3º número: ")
n4 = input("Digite o 4º número: ")
n5 = input("Digite o 5º número: ")
n6 = input("Digite o 6º número: ")
n7 = input("Digite o 7º número: ")
n8 = input("Digite o 8º número: ")
n9 = input("Digite o 9º número: ")
n10 = input("Digite o 10º número: ")


my_list = [n1, n2, n3, n4, n5, n6, n7, n8, n9 ,n10]

reversed_list = list(reversed(my_list))
print(reversed_list)

#2)>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
palavras = []

p1 = input("Escreva a 1º palavra: ")
palavras.append(p1)
p2 = input("Escreva a 2º palavra: ")
palavras.append(p2)
p3 = input("Escreva a 3º palavra: ")
palavras.append(p3)
p4 = input("Escreva a 4º palavra: ")
palavras.append(p4)
p5 = input("Escreva a 5º palavra: ")
palavras.append(p5)

palavras.sort()

print(palavras)

#3)>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
matriz = []
for i in range(3):
    linha = []
    for j in range(3):
        numero = int(input(f"Digite um número para a posição ({i},{j}):"))
        linha.append(numero)
    matriz.append(linha)

soma = 0
for linha in matriz:
    for elemento in linha:
        soma += elemento

print(f"A soma de todos os elementos da matriz é: {soma}.")

#4)>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
matriz = []
for i in range(2):
    linha = []
    for j in range(2):
        numero = int(input(f"Digite um número para a posição ({i},{j}): "))
        linha.append(numero)
    matriz.append(linha)

    transposta = [[matriz[j][i]] for j in range(2) for i in range(2)]
    print("Matriz transposta: ")
    for linha in transposta:
        print(linha)
