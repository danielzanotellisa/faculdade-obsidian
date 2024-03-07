---
tags:
  - IP
  - IPv4
  - IPv6
  - EndereçamentoDeRede
  - RedeAplicada
  - Rede
---
# Oque é
---
Os endereços locais de link para IPv4 e IPv6 são usados por um dispositivo para se comunicar com outros computadores conectados à mesma rede no mesmo intervalo de endereços IP.

A principal diferença entre o IPv4 e o IPv6 é:

- Um dispositivo IPv4 usa o endereço local do link se o dispositivo não puder obter um endereço IPv4
- Um dispositivo IPv6 deve sempre ser configurado de forma dinâmica ou manual com um endereço IPv6 local do link

## Endereço local do link IPv4

Se o seu computador windows não puder se comunicar com um servidor DHCP para obter um endereço IPv4, o Windows atribuirá automaticamente um endereço APIPA (Endereçamento Automático de IP Privado). Esse endereço de link local está no intervalo de 169.254.0.0 a 169.254.255.255.

## Endereçamento IPv6 de Link Local

Assim como o IPv4, o endereço local do link IPv6 permite que o dispositivo se comunique com outros dispositivos habilitados para IPv6 na mesma rede e somente nessa rede. Diferentemente do IPv4, todos os dispositivos habilitados para IPv6 precisam ter um endereço local de link. Os endereços locais de link IPv6 estão no intervalo de fe80:: a febf::. Por exemplo, na figura, os links para outras redes estão inativos (não conectados) como notados pelos Xs vermelhos. No entanto, todos os dispositivos na LAN ainda podem usar endereços IPv6 locais de link para se comunicarem.

![](./img/Pasted%20image%2020240301164722.png)

**NOTA:** *Diferentemente dos endereços locais de link IPv4, os endereços locais de link IPv6 são usados em uma variedade de processos, incluindo protocolos de descoberta de rede e protocolos de roteamento.
