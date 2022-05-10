NUMERO_EXERCICIOS = 3

def ler_lista_notas(n):
    """Devolve uma lista de n notas lidas do teclado"""
    lista_notas = []
    for _ in range(n):
        print("Digite a próxima nota: ")
        nota = float(input())
        lista_notas.append(nota)
    return lista_notas

def calcular_media_excluida(lista_notas, indice_excluida):
    """Devolve a média de lista_notas excluindo-se
    a nota de índice indice_excluida"""
    soma = 0.0
    for i, nota in enumerate(lista_notas):
        if i != indice_excluida:
            soma = soma + nota
    media = soma / (len(lista_notas) - 1)
    return media

def obter_indice_menor(lista_notas):
    """Devolve o índice da menor nota"""
    indice_menor = 0
    menor_nota = lista_notas[0]
    for i, nota in enumerate(lista_notas):
        if nota < menor_nota:
            menor_nota = nota
            indice_menor = i
    return indice_menor

def main():
    print("Digite as notas dos exercícios:")
    lista_notas = ler_lista_notas(NUMERO_EXERCICIOS)
    indice_menor = obter_indice_menor(lista_notas)
    media = calcular_media_excluida(lista_notas, indice_menor)
    print(f"A média excluindo a pior nota é {media}")

main()
