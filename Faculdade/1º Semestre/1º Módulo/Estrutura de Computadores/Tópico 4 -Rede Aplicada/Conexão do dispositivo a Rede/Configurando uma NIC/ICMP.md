---
tags:
  - Hardware
  - IP
  - IPv6
  - IPv4
  - Rede
  - RedeAplicada
  - TI
---
# Oque é
---
O [ICMP](https://aws.amazon.com/pt/what-is/icmp/) (Internet Control Message Protocol) é um conjunto de regras de comunicação que os dispositivos usam para informar sobre erros de transmissão de dados em uma rede, anunciar congestionamento e solucionar problemas.

Podemos por exemplo, usar o comando ***ping*** para testar a conexão entre dois computadores.

Para ver uma lista de opções que podem ser usadas, podemos digitar ***ping /?***.

![](./img/Pasted%20image%2020240304110844.png)

O ping funciona enviando uma solicitação de eco ICMP para o endereço IP digitado, caso o dispositivo que corresponde ao endereço IP digitado esteja acessível, o dispositivo receptor retornará uma mensagem de resposta de eco ICMP para confirmar a conectividade.

É possível usar o ***ping*** para testar conectividade com um site digitando o nome de domínio. O computador primeiro usará o DNS para encontrar o endereço IP e depois enviar a solicitação de eco ICMP para esse endereço IP.

![](./img/Pasted%20image%2020240304111126.png)

