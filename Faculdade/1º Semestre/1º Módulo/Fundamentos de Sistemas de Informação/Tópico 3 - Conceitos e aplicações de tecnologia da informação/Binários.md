---
tags:
  - binarios
  - SI
  - Hardware
  - TI
  - software
  - sistemasDeInformação
---
# Oque é:
---

No sistema **BINÁRIO** vamos chamar cada um de seus símbolos de BIT (BInary digiT). Assim, teremos 2 bits: 0 e 1.

Ao agrupar 8 bits temos um **BYTE**

Logo: 

1 bit -> 0 ou 1

1 byte --> 8 bits --> sequência de 8 bits (11100101).


Porém, representar números muito grandes pode ser um problema, para isso, podemos usa um sistema de numeração de base 16, ou [[Hexadecimais|hexadecimal]].


## Convertendo um decimal para binário
---

Para realizarmos a conversão de um decimal para binário, nós iremos dividir o nosso número por 2, pegando os seus restos até que o dividendo tenhamos quociente 0.
Vamos pegar por exemplo o número 8:

8/2 = 4 resto 0
4/2 = 2 resto 0
2/2 = 1 resto 0

Logo teremos o binário --> 1000 para representar o 8

Outro exemplo com o número 57:

57/2 = 28 resto 1
28/2 = 14 resto 0
14/2 = 7 resto 0
7/2 = 3 resto 1
3/2 = 1 resto 1

Binário correspondente --> 111001

Para converter um número binário para decimal, basta pegar a posição que corresponde ao digito sempre contando da direita pra esquerda e multiplicar o digito x 2elevado a posição.

No caso do 111001 ficaria

Posição:543210

Bit:        111001

Logo --> $1x2^5+1x2^4+1x2^3+0x2^2+0x2^1+1x2^0=57$

