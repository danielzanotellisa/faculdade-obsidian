#virtualização #Hardware #EstruturaDeComputadores #Servidores 

# Conceito
---
Um hypervisor é também conhecido como Virtual Machine Manager (VMM), é o cérebro da virtualização. O hypervisor é o software responsável por criar e gerenciar VMs.

Ele aloca os recursos físicos do sistema, conforme necessário. Isso garante que a operação de uma VM não interfira na outra.

## Tipos de Hipervisores

1. <span style="color:#d97f36">Hypervisor tipo 1 (bare-metal)</span> - ele tem acesso direto aos recursos do hardware, a máquina host não tem um sistema operacional instalado em uma configuração de hypervisor bare-metal. O software do hypervisor atua como um sistema operacional leve.
2. <span style="color:#d97f36">Hypervisor tipo 2 (hospedado)</span> - hospedado por um sistema operacional e normalmente é usado como virtualização do lado do cliente. 

Os hipervisores tipo 1 são comuns em data centers e na computação em nuvem. Os exemplos de hipervisores tipo 1 incluem ⁪VMware VSphere/ESXi, Xen e Oracle servidor VM.

Os hipervisores tipo 2, como VMware Estação de trabalho, funcionam com o computador host para criar e usar várias VMs. O Windows Hyper-V também está incluído no Windows 10 pro e no Windows Server (2012 e 2016).

![](img/Pasted%20image%2020240313154013.png)
