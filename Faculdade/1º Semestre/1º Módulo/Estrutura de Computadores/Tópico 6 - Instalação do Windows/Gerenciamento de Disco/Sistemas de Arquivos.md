#SIstemaOperacional #Windows #EstruturaDeComputadores #Hardware 


# Tipos de sistemas de arquivos
---

- <span style="color:#d97f36">FAT32</span> (File Allocation Table, 32bits): compatível com partições de até 2TB. O sistema de arquivos FAT32 é usado pelo Windows XP e por versões anteriores do sistema operacional
- <span style="color:#d97f36">NTFS</span>(New Technology File System): na teoria, compatível com partições até 16 hexabytes. O NTFS incorpora recursos de segurança para sistemas de arquivos e atributos estendidos. O Windows 8.1, Windows 7 e Windows 10 criam automaticamente uma partição usando todo o disco rígido. Se um usuário não criar partições personalizadas usando a opção Novo, como mostrado na figura, o sistema formatará a partição e iniciará a instalação do Windows. Se o usuário criar uma partição, ele poderá determinar o tamanho dela.
- <span style="color:#d97f36">exFAT</span>(FAT 64): criado para solucionar algumas limitações dos sistemas FAT, FAT32 e NTFS ao formatar pendrives USB, como por exemplo, o tamanho dos arquivos e o tamanho dos diretórios. Uma das principais vantagens do exFAT é a compatibilidade com arquivos com tamanho superior a 4 GB.
- <span style="color:#d97f36">CDFS</span> **(Compact Disc File System, Sistema de arquivos para CD)**: criado especificamente para mídias de disco óptico.
- <span style="color:#d97f36">NFS</span> **(Network File System, Sistema de Arquivos de Rede)**: sistema de arquivos em rede que permite o acesso a arquivos pela rede. Do ponto de vista do usuário, não há diferença entre acessar um arquivo armazenado localmente ou em outro computador na rede. O NFS é um padrão aberto, o que permite que qualquer pessoa o implemente.

## Formatação Rápida vs Completa
---

O formatação rápida remove os arquivos da partição, mas não verifica se há setores defeituosos no disco. Verificar o disco em busca de setores defeituosos pode evitar a perda de dados no futuro.

A formatação completa remove os arquivos da partição e, ao mesmo tempo, examina o disco em busca de setores defeituosos. Ela é necessária para todos os discos rígidos novos. A opção de formatação completa leva mais tempo para ser concluída.