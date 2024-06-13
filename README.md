# DIO - Trilha Java Básico
www.dio.me

#### Autores
- [Gleyson Sampaio](https://github.com/glysns)

## Desenvolvedora da solução: 
- [Rutiele Rios](https://github.com/Rutiele93)

## Controle de Fluxo - Desafio Proposto

Vamos exercitar todo o conteúdo apresentado no módulo de Controle de Fluxo codificando o seguinte cenário.

O sistema deverá receber dois parâmetros via terminal que representarão dois números inteiros, com estes dois números você deverá obter a quantidade de interações (for) e realizar a impressão no console (System.out.print) dos números incrementados, exemplo:

* Se você passar os números 12 e 30, logo teremos uma interação (for) com 18 ocorrências para imprimir os números, exemplo: `"Imprimindo o número 1"`, `"Imprimindo o número 2"` e assim por diante.
* Se o primeiro parâmetro for MAIOR que o segundo parâmetro, você deverá lançar a exceção customizada chamada de `ParametrosInvalidosException` com a segunda mensagem: "O segundo parâmetro deve ser maior que o primeiro"   


1. Crie o projeto `DesafioControleFluxo`
2. Dentro do projeto, crie a classe `Contador.java` para realizar toda a codificação do nosso programa.
3. Dentro do projeto, crie a classe `ParametrosInvalidosException` que representará a exceção de negócio no sistema. 

# Lógica da Solição do desafio

Este projeto é uma aplicação Java simples que demonstra o controle de fluxo utilizando loops e exceções customizadas. A aplicação recebe dois parâmetros inteiros via terminal, valida os parâmetros e, se válidos, imprime uma sequência de números.

### Lógica do Projeto
#### 1. Leitura dos Parâmetros:

- A aplicação solicita ao usuário que insira dois números inteiros: parametroUm e parametroDois.
- Esses números são lidos utilizando a classe Scanner.

#### 2. Validação dos Parâmetros:

- O programa verifica se parametroUm é maior ou igual a parametroDois.
- Se essa condição for verdadeira, uma exceção customizada chamada ParametrosInvalidosException é lançada com a mensagem: "O segundo parâmetro deve ser maior que o primeiro".

#### 3. Contagem e Impressão:

- Se os parâmetros forem válidos, o programa calcula a diferença entre parametroDois e parametroUm, que determina a quantidade de iterações necessárias.
- Um loop for é utilizado para imprimir os números incrementados, começando de 1 até a quantidade de iterações calculadas.

### Estrutura do Código
O projeto consiste em duas classes principais:

#### - ParametrosInvalidosException:

- Esta classe é uma exceção customizada que estende Exception.
- Utilizada para sinalizar que o segundo parâmetro é menor ou igual ao primeiro.
#### - Contador:

- Contém o método main para a execução do programa.
- Lê os parâmetros do usuário, valida os parâmetros e, se válidos, chama o método contar para realizar a contagem e impressão dos números.


### Como Executar
```sh
Clone o repositório do projeto. https://github.com/Rutiele93/Dio-Desafio-Contador-de-Fluxo.git
cd CONTROLEDEFLUXO
```
- Compile as classes Java.
- Execute a classe Contador e insira os dois números inteiros conforme solicitado.
- O programa validará os parâmetros e, se válidos, imprimirá a sequência de números.

### Exemplo de Uso
Se você inserir 12 como o primeiro parâmetro e 30 como o segundo parâmetro:
O programa imprimirá os números de 1 a 18.
Se você inserir 30 como o primeiro parâmetro e 12 como o segundo parâmetro:
O programa lançará uma exceção com a mensagem "O segundo parâmetro deve ser maior que o primeiro".
