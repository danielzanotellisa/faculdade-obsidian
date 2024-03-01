---
tags:
  - EndereçamentoDeRede
  - Rede
  - RedeAplicada
  - IP
---
# Oque é
---

É o endereço que permite que dispositivos se comuniquem com outros que estão na mesma ou em diferente redes através de um roteador. Possuem 32bit representados em decimais. Os 32 bits são divididos em 8 partes, 3 com 3 dígitos e uma com 1 dígito. Ex: 192.168.1.100

Cada conjunto de de numero representa 8 bits.

Os IPv4 tem um "[subnet mask](https://nordvpn.com/pt-br/blog/mascara-de-sub-rede/)" que serve para separar os endereços IP em partes de rede e host. Ao definir quantos bits do endereço IP representam a parte da rede e quantos bits representam a parte do host, ela ajuda no gerenciamento e desempenho do tráfego. 

As mascaras de sub-rede possuem um valor específico sendo ele todos 1s e o resto dos 32 bits sendo um 0. Ex: 255.255.255.0

Através de uma máscara de sub-rede (subnet) é possível segmentar redes grandes em redes menores, favorecendo o um fluxo e um tráfego de informações mais dinâmico, evitando sobrecarga nos servidores e na rede em si.

Elas podem ser representadas usando o "/" seguido do numero de bits com valor 1. 
   - 255.255.255.0 --> /24 

192 . 168 .   1 . 100
255 . 255 . 255 . 0

No exemplo acima, os 24bits de 255 representam a parte da rede, e o os 8 bits de 0 representam o host.
