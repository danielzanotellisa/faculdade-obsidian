---
tags:
  - Hardware
  - hexdecimal
  - SI
  - sistemasDeInformação
  - TI
  - software
---

# Oque é
---

Assim como os [[Binários|binários]], os hexadecimais são uma sistema de numeração.

Nesse caso usamos uma base 16 para representar números muito grandes.

![](./img/Pasted%20image%2020240228154731.png)

## Convertendo um decimal para hexadecimal
---

Para realizar essa conversão basta dividirmos o numero por que queremos por 16 e alinharmos os seus restos até que os restos sejam 0 ou o número n seja mais divisível por 16.
![](./img/Pasted%20image%2020240228162233.png)
Caso o resto seja MAIOR que 9, usaremos a letra correspondente a ele, representado na tabela acima.

3798 para hexadecimal:

- 3798/16 = 237 resto 6
- 237/16 = 14 resto 13
- 14/16 = 0 resto 14

Logo, temos o número hexadecimal 0ED6.


Para convertermos esse número de volta para decimal basta fazermos da mesma forma que fizemos com os binários, só que, ao invés da base ser 2, vai ser 16

$$
0x16^3 + 14x16^2 + 13x16^1 + 6x16^0 = 3798
$$

Para realizar essa conversão, nós iremos assimilar o as **letras** de volta aos números q elas repressentam