---
tags:
  - EndereçamentoDeRede
  - Rede
  - RedeAplicada
  - IP
---
# Oque é
---

É o endereço que permite que dispositivos se comuniquem com outros que estão na mesma ou em diferente redes através de um roteador. 

Os IPv4 tem um "[subnet mask](https://nordvpn.com/pt-br/blog/mascara-de-sub-rede/)" que serve para separar os endereços IP em partes de rede e host. Ao definir quantos bits do endereço IP representam a parte da rede e quantos bits representam a parte do host, ela ajuda no gerenciamento e desempenho do tráfego. 

As mascaras de sub-rede possuem um valor específico sendo ele todos 1s e o resto dos 32 bits sendo um 0. Ex: 255.255.255.0

Através de uma máscara de sub-rede (subnet) é possível segmentar redes grandes em redes menores, favorecendo o um fluxo e um tráfego de informações mais dinâmico, evitando sobrecarga nos servidores e na rede em si.

Elas podem ser representadas usando o "/" seguido do numero de bits com valor 1. 
   - 255.255.255.0 --> /24 

192 . 168 .   1 . 100
255 . 255 . 255 . 0

No exemplo acima, os 24bits de 255 representam a parte da rede, e o os 8 bits de 0 representam o host.

Formato de um endereço IPv4:

![[Pasted image 20240301155832.png]]


Quando configuramos manualmente um dispositivo com um endereço IPv4, usamos o formato decimal. Cada número separado por um ponto é chamado de octeto porque representa 8 bits.

Sabemos que o endereço IPv4 é composto por duas partes: a primeira que identifica a rede em e a segunda que identifica o dispositivo dentro dessa rede

A mascara de sub-rede é usada pelo dispositivo para determinar a rede.

![[Pasted image 20240301162210.png]]

![[Pasted image 20240301161715.png]]

No exemplo acima, a parte da rede é composta pelos 3 primeiros octetos: 192.168.200 enquanto o dispositivo é identificado pelo ultimo octeto: ".8", essa é a parte exclusiva desse dispositivo na rede 192.168.200.0.

Qualquer outro dispositivo com o mesmo prefixo estará na mesma rede.

Quando o dispositivo prepara dados para enviar para rede, ele deve primeiro determinar se os dados devem ser enviados diretamente para o receptor pretendido ou para um [[Roteadores|roteador]].

Caso o dispositivo que irá receber os dados esteja em OUTRA rede, os dados serão enviados para um roteador, e o roteador irá encaminhar os dados para a rede correta. 