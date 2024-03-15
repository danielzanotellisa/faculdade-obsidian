#Hardware #SIstemaOperacional #Windows #EstruturaDeComputadores 


# Oque é
---

O particionamento de uma unidade de armazenamento nada mais é do que a divisão dela para que cada parte possa armazenar informações.

Particionar é um processo simples, porém, para garantir uma inicialização correta, é necessário informar ao firmware em qual partição e qual disco o SO se encontra instalado

Dois padrões populares de esquema de partição:

<span style="color:#d97f36">Master Boot Record</span> (MBR)

- Introduzido publicamente em 1983, o MBR contém informações sobre como as partições do disco rígido são organizadas. Tem 512 bytes de tamanho e contém o carregador de boot, um programa executável que permite que o usuário escolha entre várias opções de sistemas operacionais. O MBR se tornou o padrão de fato, mas ele tem limitações que precisavam ser abordadas. Ele é comumente usado em computadores com firmware baseado em BIOS.

<span style="color:#d97f36">Tabela de partição GUID</span> 

- Também projetada como um esquema de tabela de partição padrão para discos rígidos, a GPT utiliza várias técnicas modernas para expandir o esquema de particionamento MBR mais antigo. A GPT é comumente usada em computadores com firmware de UEFI. Atualmente, a maioria dos sistemas operacionais modernos é compatível com a GPT.

![](img/Pasted%20image%2020240315145105.png)

