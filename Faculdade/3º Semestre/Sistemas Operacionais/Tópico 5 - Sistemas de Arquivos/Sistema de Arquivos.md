---
tags:
  - Linux
  - SIstemaOperacional
  - Desenvolvimento
---
---

## Componentes básicos de um sistema de arquivos
---
- Todos os sistemas de arquivos em um dispositivo de armazenamento físico são essencialmente divididos em duas regiões principais: a área de controle e a área de dados
	- Área de controle: Contém todas as informações sobre a estrutura do sistema de arquivos, como tabelas de alocação, metadados de arquivos, informações de diretório etc.
	- Área de dados: O corpo do sistema de arquivos, onde os próprios dados são armazenados fisicamente
- Metadados são as informações de um determinado arquivo, como hora e data de criação, permissões, tamanho, proprietário e grupo.
- Em um sistema de arquivos temos os blocos e os buffers
	- Blocos são usados para dividir o espaço de armazenamento, essa divisão facilita a alocação de espaço e gestão de armazenamento. Geralmente, os blocos tem um tamanho de 4KB
	- Buffers é uma área temporária de armazenamento, geralmente na memória RAM, usada para armazenar dados temporariamente enquanto são transferidos entre duas áreas, especialmente quando essas áreas operam a diferentes velocidades. O uso do buffer serve para melhor o desempenho na cópia/conversão de arquivos, pois lida com a discrepância de velocidade entre a leitura e a escrita

## Inodes e diretórios
---

- Um inode é uma estrutura de dados fundamental em sistemas de arquivos. Ele atua como um ponto de referência para arquivos e diretórios, contendo metadados sobre eles, exceto seu nome e conteúdo real.
- Cada arquivo ou diretório em um sistema UNIX/Linux tem um inode associado que contém informações como:
	- Tamanho do arquivo
	- Dispositivo no qual o arquivo está armazenado
	- Permissões de acesso ao arquivo
	- Horários de criação, modificação e acesso
	- Tipo de arquivo(regular, diretório, link simbólico, etc)
	- Contagem de links(número de hard links para o arquivo)
	- Localização dos blocos de dados do arquivo no disco(ponteiros para os blocos de dados)
- 