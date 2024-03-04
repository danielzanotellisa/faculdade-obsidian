---
tags:
  - Hardware
  - Configuração
  - RedeAplicada
  - Rede
  - TI
  - IPv6
  - IPv4
  - IP
---
# Instruções
---

# Exibir padrões da WLAN

- Os roteadores sem fio já são configurados para fornecer acesso sem fio a dispositivos utilizando um nome de rede sem fio padrão e senha. 
- O nome de uma rede sem fio é chamado de SSID(Service Set Identified). 

![[Pasted image 20240304135928.png]]

## Alterar modo de rede

- Podemos alterar qual padrão 802.11 implementar. Podemos selecionar um padrão específico, ou deixar vários ao mesmo tempo.
- Selecionar um ou dois padrões pode fazer com que você tenha um desempenho melhor de rede.

![[Pasted image 20240304140058.png]]

## Configure a SSID

- Podemos atribuir um SSID à LAN sem fio, o roteador comunicará sua presença enviando broadcasts que anunciam seu SSID. Isso permitirá que hosts sem fio descubram automaticamente o nome da rede sem fio
- Se a transmissão de SSID estiver desativada, devemos inserir manualmente o SSID nos dispositivos sem fio que conectam a WLAN.

![[Pasted image 20240304141016.png]]

## Configure o canal

- Os dispositivos configurados com o mesmo canal na faixa de 2,4GHz podem se sobrepor e causar distorção, diminuindo o desempenho sem fio e potencialmente interrompendo as conexões de rede. A solução para isso é configurar canais não sobrepostos.
- Alguns roteadores tem a opção de que o aparelho selecione a melhor opção automaticamente.

![[Pasted image 20240304141214.png]]

## Configurar o modo de segurança

- Na configuração padrão, o roteador sem fio pode não ter nenhuma segurança WLAN.

![[Pasted image 20240304141317.png]]

- na imagem acima, a versão pessoal do Wi-Fi Protected Access versão 2 (WPA2 Personal) está selecionada junto com a criptografia AES(Advanced Ecryption Standard) que atualmente é o modo de segurança mais forte.

## Configure a senha

- O WPA2-Personal usa uma senha para autenticar clientes sem fio. WPA2 é mais fácil de ser utilizado em pequenos escritórios e residências pois não requer um servidor de autenticação.
- Organizações maiores implementam a WPA2-Enterprise e precisam que os clientes sem fio se autentiquem com nome de usuário e senha.

![[Pasted image 20240304141555.png]]

