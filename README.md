# Projeto_Calculadora
Calculadora criada na aula da Ebac


# Calculadora Básica

Este é um projeto simples em Python que implementa uma calculadora básica com as operações de adição, subtração, multiplicação e divisão. Além disso, permite ao usuário encerrar o programa.


## **Funcionalidades**

1. Solicita ao usuário dois números como entrada.
2. Exibe um menu com as seguintes opções:
   - Adição
   - Subtração
   - Multiplicação
   - Divisão
   - Sair
3. Realiza a operação escolhida e exibe o resultado.
4. Trata casos de divisão por zero com uma mensagem de erro.
5. Permite sair do programa ao selecionar a opção correspondente.

## **Explicação do Código Python**

O código é estruturado da seguinte forma:

1. **Entrada de números**:
   - Solicita ao usuário dois números.
   ```python
   num1 = float(input("Digite o primeiro número: "))
   num2 = float(input("Digite o segundo número: "))
   ```

2. **Exibição do menu de operações**:
   - Apresenta as opções disponíveis para o usuário.
   ```python
   print("\nQual operação matemática deseja fazer?")
   print("1. Adição")
   print("2. Subtração")
   print("3. Multiplicação")
   print("4. Divisão")
   print("5. Sair")
   ```

3. **Execução da operação escolhida**:
   - Baseado na escolha do usuário, realiza a operação correspondente.
     - **Adição**:
       ```python
       resultado = num1 + num2
       print(f"Resultado da adição: {resultado}")
       ```
     - **Subtração**:
       ```python
       resultado = num1 - num2
       print(f"Resultado da subtração: {resultado}")
       ```
     - **Multiplicação**:
       ```python
       resultado = num1 * num2
       print(f"Resultado da multiplicação: {resultado}")
       ```
     - **Divisão**:
       - Verifica se o divisor não é zero antes de calcular:
       ```python
       if num2 != 0:
           resultado = num1 / num2
           print(f"Resultado da divisão: {resultado}")
       else:
           print("Erro: Divisão por zero não é permitida.")
       ```
     - **Sair**:
       - Exibe uma mensagem e encerra o programa.
       ```python
       print("Saindo do programa.")
       ```

4. **Tratamento de escolha inválida**:
   - Caso o usuário insira uma opção não listada, uma mensagem de erro é exibida.
   ```python
   print("Escolha inválida. Tente novamente.")
   ```

## **Execução do Programa**

Para executar o programa, siga os passos abaixo:

### **Com o arquivo Python (.py)**
1. Certifique-se de ter o Python 3 instalado na sua máquina.
2. Abra o terminal ou prompt de comando e navegue até a pasta onde o arquivo `Calculadora_basica.py` está salvo.
3. Execute o comando:
   ```bash
   python3 Calculadora_basica.py
   ```

### **Com o arquivo .sh**
1. Certifique-se de ter o Python 3 instalado na sua máquina.
2. Abra o terminal e navegue até a pasta onde o arquivo `executar_calculadora.sh` está salvo.
3. Torne o arquivo executável com o comando:
   ```bash
   chmod +x executar_calculadora.sh
   ```
4. Execute o script:
   ```bash
   ./executar_calculadora.sh
   ```
