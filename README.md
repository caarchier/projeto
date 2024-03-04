def soma(x, y):
    return x + y

def subtracao(x, y):
    return x - y

def multiplicacao(x, y):
    return x * y

def divisao(x, y):
    if y == 0:
        return "Erro! Divisão por zero não é permitida."
    else:
        return x / y

def main():
    print("Bem-vindo à Calculadora!")

    while True:
        print("\nOperações disponíveis:")
        print("1. Adição")
        print("2. Subtração")
        print("3. Multiplicação")
        print("4. Divisão")
        print("5. Sair")

        escolha = input("Escolha uma operação (1/2/3/4/5): ")

        if escolha in ('1', '2', '3', '4'):
            num1 = float(input("Digite o primeiro número: "))
            num2 = float(input("Digite o segundo número: "))

            if escolha == '1':
                print("Resultado:", soma(num1, num2))
            elif escolha == '2':
                print("Resultado:", subtracao(num1, num2))
            elif escolha == '3':
                print("Resultado:", multiplicacao(num1, num2))
            elif escolha == '4':
                print("Resultado:", divisao(num1, num2))
        elif escolha == '5':
            print("Saindo da calculadora...")
            break
        else:
            print("Opção inválida! Por favor, escolha uma opção válida.")

if __name__ == "__main__":
    main()
