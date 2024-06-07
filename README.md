def calcular():
    print("Bem-vindo à Calculadora Python")

    while True:
        operacao = input("Escolha a operação (somar, subtrair, multiplicar, dividir) ou 'sair' para encerrar: ").lower()

        if operacao == 'sair':
            print("Obrigado por usar a Calculadora Python. Até logo!")
            break

        if operacao not in ('somar', 'subtrair', 'multiplicar', 'dividir'):
            print("Operação inválida")
            continue

        num1 = float(input("Digite o primeiro número: "))
        num2 = float(input("Digite o segundo número: "))

        if operacao == 'somar':
            resultado = num1 + num2
            print(f"O resultado da soma é {resultado}")
        elif operacao == 'subtrair':
            resultado = num1 - num2
            print(f"O resultado da subtração é {resultado}")
        elif operacao == 'multiplicar':
            resultado = num1 * num2
            print(f"O resultado da multiplicação é {resultado}")
        elif operacao == 'dividir':
            if num2 != 0:
                resultado = num1 / num2
                print(f"O resultado da divisão é {resultado}")
            else:
                print("Erro: Divisão por zero não é permitida.")

if __name__ == "__main__":
    calcular()
