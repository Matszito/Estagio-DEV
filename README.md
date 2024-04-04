```
1) Observe o trecho de código abaixo:

int INDICE = 13, SOMA = 0, K = 0;
enquanto K < INDICE faça
{
    K = K + 1;
    SOMA = SOMA + K;
}
imprimir(SOMA);

Ao final do processamento, qual será o valor da variável SOMA?
Resposta: Ao final do processamento o valor da variavel SOMA será 91


2) Dado a sequência de Fibonacci, onde se inicia por 0 e 1 e o próximo valor sempre será a soma dos 2 valores anteriores (exemplo: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34...), escreva um programa na linguagem que desejar onde, informado um número, ele calcule a sequência de Fibonacci e retorne uma mensagem avisando se o número informado pertence ou não a sequência.
Resposta: Eu utilizei python, pois é uma linguagem que estou estudando sobre.

def fibonacci(n):
    intZero = 0
    intUm = 1

    while intUm < n:
        intZero, intUm = intUm, intZero + intUm
    #

    return intUm == n
#

intNumero = int(input("Digite um número: "))
blFibonacci = fibonacci(intNumero)

if blFibonacci:
    print("O número informado pertence a sequência de Fibonacci")
else:
    print("O número informado não pertence a sequência de Fibonacci")
#


3) Descubra a lógica e complete o próximo elemento:
a) 1, 3, 5, 7, 9
b) 2, 4, 8, 16, 32, 64, 128
c) 0, 1, 4, 9, 16, 25, 36, 49
d) 4, 16, 36, 64, 100
e) 1, 1, 2, 3, 5, 8, 13
f) 2,10, 12, 16, 17, 18, 19, 200



4) Você está em uma sala com três interruptores, cada um conectado a uma lâmpada em uma sala diferente. Você não pode ver as lâmpadas da sala em que está, mas pode ligar e desligar os interruptores quantas vezes quiser. Seu objetivo é descobrir qual interruptor controla qual lâmpada.
Como você faria para descobrir, usando apenas duas idas até uma das salas das lâmpadas, qual interruptor controla cada lâmpada?
Resposta: Você liga o primeiro interruptor e deixa ele ligado alguns minutos, após isso você liga o segundo interruptor.
Em seguida você verifica a sala que está com a lâmpada acessar, essa é ligada pelo segundo interruptor, após você verifica a lampada de outra sala, se ela estiver fria, significa que aquela lâmpada é do terceiro interruptor e a sala que sobrou se refere ao primeiro interruptor, se estiver quente é o contrario.

 

5) Escreva um programa que inverta os caracteres de um string.
Resposta: Eu utilizei python novamente.

def inverter(texto):

    strTextoInvertido = ''
    intTextoSize = len(texto)

    while intTextoSize > 0:
        strTextoInvertido += texto[intTextoSize - 1]
        intTextoSize -= 1
    #

    return strTextoInvertido
#

texto = input('Digite um texto: ')
print(inverter(texto))
```
