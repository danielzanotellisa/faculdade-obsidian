---
tags:
  - hexdecimal
  - IP
  - EndereçamentoDeRede
  - Rede
  - RedeAplicada
---
# Oque é
---
O IPv6 veio para substituir a versão 4, permitindo que uma demanda maior de dispositivos pudessem se conectar a internet.

Os endereços IPv6 são constituídos por 8 blocos de 16 bits cada,128bits no total, que são separados pelo caractere ":". Cada um desses grupos de 16bits conta com 4 símbolos hexadecimais que podem ir de 0000 a FFFF.

Exemplo de um endereço IPv6: 2001:BB6:AD:F:0:0:0:1

Podemos comprimir esse endereço usando duas regras:

  - Os Zeros iniciais de cada segmento de 16 bits podem ser omitidos
  - Um segmento que houver apenas 0s pode ser substituído por "::"

Semelhante ao IPv4, o IPv6 também usa a notação prefixa com o "/" para indicar a porção da rede e a do host

2001:db8:acad:100:37ef:100:a765:1/64

O "/64" representa os 4 primeiros segmentos que são a porção da rede.

Todos os dispositivos conectados na mesma rede vão compartilhar o mesmo prefixo de IPv6.

Formato de um endereço IPv6:

![[Pasted image 20240301155921.png]]

