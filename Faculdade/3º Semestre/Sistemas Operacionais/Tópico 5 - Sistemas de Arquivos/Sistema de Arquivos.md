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
- O inode não armazena o nome ou conteúdo real de um arquivo, esse trabalho é o do diretório, que aponta para o inode correspondente. A princípio os diretórios podem parecer somente containers para guardar arquivos, mas em sistemas UNIX eles são na verdade arquivos especiais que contêm listas de entradas associando nomes de arquivos a seus inodes. Quando um usuário acessa um diretório e vê a lista de arquivos, está na verdade olhando para o conteúdo desse arquivo de diretório.
- Para entender como os diretórios funcionam precisamos também entender hard e soft (symbolic) links.
	- Hard Link: Funciona como uma "cópia", criamos um link que aponta para o mesmo inode do arquivo inicial. Qualquer alteração feita em um hard link será refletido no arquivo original, afinal, estamos alterando o conteúdo no mesmo espaço de memória do arquivo original. Ao deletarmos o arquivo original, o hard link ainda funcionará. Algo só pode ser deletado da memória quando deletamos todos os hard links que apontam para o conteúdo.
	- Soft Link: É uma referência ao nome do arquivo e não ao seus dados. Um arquivo separado que aponta para outro arquivo. Se o arquivo original for excluído, o soft link não irá mais funcionar. Possuem seu próprio inode e podem ser identificados como *links simbólicos* em listagens de diretórios
	- Podemos criar um hard link usando o comando: `ln <arquivo_para_ser_linkado> [nome do arquivo]`
	- Para criarmos um soft link usamos a seguinte sintaxe: ```ln -s <nome_do_arquivo_para_vincular_o_link> [nome do novo arquivo link]```
## Manipulação de arquivos
---

- 
