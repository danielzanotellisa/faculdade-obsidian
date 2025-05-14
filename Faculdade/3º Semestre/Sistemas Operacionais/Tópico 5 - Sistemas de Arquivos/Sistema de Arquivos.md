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

- A manipulação de arquivos e diretórios em sistemas UNIX/Linux é feita majoritariamente atráves da linha de comando.
	- Comandos uteis para se gravar:
		- **touch**: cria um arquivo no diretório atual
		- **rm `<nome do arquivo>`**: remove o arquivo especificado (não exclui completamente os dados, apenas libera o espaço na memória para que outras coisas possam ser alocadas ali)
		- **wipe**: usado para destruir de forma segura o conteúdo de um arquivo, garantindo que ele não possa ser recuperado
		- **file**: determina o tipo de arquivo observando os padrões de dados dentro do arquivo
		- **foremost**: ferramenta de recuperação de dados que busca por assinaturas ou padrões de arquivo específicos.
		- **stat**: serve para visualizarmos metadados como: inode, proprietário do arquivo, grupo do arquivo e o MAC time:
			- Modified: hora em que o arquivo foi modificado pela última vez
			- Acessed: hora em que o arquivo foi acessado pela última vez
			- Changed: hora em que os metadados do arquivo foram alterados pela última vez
- A persistência dos dados refere-se à capacidade dos dados de permanecerem em um dispositivo, mesmo depois de aparentemente terem sido excluídos ou, em alguns casos, após o dispositivo ter sido formatado.
- A formatação é o processo de preparação de um dispositivo de armazenamento para ser usado por um sistema de arqvuios. Durante a formatação, a estrutura e os diretórios do sistema de arquivos são criados.
	- Uma formatação simples não apaga completamente os dados do sistema, ela apenas apaga as referências aos dados e marca o espaço como disponível. Mesmo que o dispositivo pareça estar vazio, os dados originais ainda podem persistis nele até serem sobrescritos.

## Fragmentação
---

- A fragmentação pode ocorrer de dudas formas, em arquivos ou na unidade de armazenamento:
	- Arquivos: Quando o arquivo é muito grande e não pode ser armazenado em um pedaço contíguo de memória, ele é fragmentado para que possa caber na unidade de armazenamento. Isso faz com que a leitura e a escrita desse arquivo se torne mais lenta, pois o sistema operacional e a unidade de armazenamento tem de buscar por esse arquivo em blocos de memória separados.
	- Fragmentação de espaço: Pode ocorrer após a exclusão e gravação repetida de arquivos, esse tipo de fragmentação pode impedir a criação de arquivos maiores que, de outra forma, caberiam no espaço total não utilizado disponível, simplesmente porque esse espaço não está contíguo. Para isso existe a desfragmentação, que reorganiza os arquivos para que eles ocupem um espaço de memória contíguo, melhorando assim o desempenho na leitura e gravação de novos arquivos.
		- A desfragmentação é muito útil para unidades em disco mas pouco útil para SSDs, ja que eles usam memórias flash (não é recomendado a desfragmentação pois isso acaba com a vida útil dos SSDs). Para os SSDs, é recomendado o trim, um comando que permite que o sistema operacional informe ao SSD quais blocos de dados não são mais considerados em uso e podem ser apagados internamente.

## Tipos de alocação
---

- Existem vários métodos e tipos de alocação de dados diferentes. Entender como elas funcionam é essencial.
- Procurar mais detalhes sobre as alocações encadeadas (FAT), alocação indexada (NTFS ou ext4), B-tree etc etc.
- A técnica de alocação adotada pelo sistema de arquivos influencia diretamente a eficiência na utilização e gestão do espaço em disco, assim como no desempenho de leitura e gravação de arquivos. Cada abordagem apresenta vantagens e desvantagens, e a escolha ideal frequentemente varia de acordo com os requisitos específicos do sistema e as características predominantes de uso.

## Virtual File System (VFS)
---
- Oferece um conjunto de abstrações que torna a comunicação entre aplicativos e usuários com os diversos sistemas de armazenamento de arquivos mais fácil
- Como se fosse um intermediador, ele reune todos os arquivos que podem estar espalhados em unidades de armazenamento diferentes em uma única "árvore" de forma abstrata para que o acesso seja facilitado
- Pode realizar o caching de inode e de diretório para acelerar o acesso aos sistemas de arquivos
- Apresenta uma arquitetura modular oque torna relativamente simples adicionar suporte a novos sistemas de arquivos
- Pode implementar verificações de segurança e outras políticas, garantindo que os aplicativos não violem as regras de acesso ao tentar ler ou escrever em sistemas de arquivos

## Tipos de Sistema de Arquivos
---

- Escolher um sistema de arquivos adequado depende em grande parte das necessidades do usuário, do tipo de dispositivo de armazenamento e do ambiente operacional específico
- Alguns tipos de sistema de arquivos são:
	- FAT
	- FAT32
	- FAT64
	- NTFS
	- EXT2/3/4

## Jornalamento e Integridade
---

- O *logging* é um "jornal" onde as operações de escrita que estão prestes a serem realizadas são escritas. Serve para que em caso de reinicializações, desligamentos ou falhas de hardware/software abruptas, o sistema possa saber de onde parou para dar continuidade ou reverter a um ponto seguro todos os arquivos que estavam sendo utilizados.
- Garante (não 100%) a integridade de arquivos e sua consistênca.
- Existem tipos de "jornalamento"
	- journal: todas as informações como metadados e conteúdo são gravadas no jornal antes de serem escritas no local de armazenamento
	- ordered: somente os metadados são gravados no jornal mas eles são escritos antes dos dados associados
	- writeback: apenas os metadados são jornalados e não há ordem específica garantida para a escrita de dados reais
