#EstruturaDeComputadores #SIstemaOperacional #Linux #macOS 


# Permissões básicas
---

- O Unix usa permissões de arquivo para reforçar os limites dentro do sistema
- As permissões são incorporadas à estrutura do sistema de arquivos e fornecem um mecanismo para definir permissões para todos os arquivos e diretórios
- Todo arquivo e diretório nos sistemas Unix carregam suas permissões que definem as ações que o proprietário, o grupo e outras pessoas podem realizar com o arquivo ou diretório
- O usuário root é o único que se sobrepõe às permissões
	- Ele pode realizar escrita em qualquer arquivo
	- Como tudo é tratado como arquivo, o usuário root tem controle total do sistema operacional
	- O acesso como root é muitas vezes necessário antes de realizar tarefas administrativas e de manutenção

## Valores de Permissão

![](../../img/Pasted%20image%2020240325132837.png)

![](../../img/Pasted%20image%2020240325132850.png)

- <span style="color:#d97f36">777 (-rwxrwxrwx)</span> - Não há restrições, qualquer um pode ler, gravar ou executar o arquivo
- <span style="color:#d97f36">755 (-rwxr-xr-x)</span> - O proprietário tem todas as permissões, os outros só podem ler e executar o arquivo
- <span style="color:#d97f36">700 (-rwx------)</span> - Somente o proprietário pode ler, gravar ou executar o arquivo
- <span style="color:#d97f36">666 (-rw-rw-rw-)</span> - Todos podem somente ler e gravar o arquivo mas não executar
- <span style="color:#d97f36">644 (-rw-r--r--)</span> - Somente o proprietário pode ler e gravar o arquivo, os outros usuários só podem fazer a leitura
- <span style="color:#d97f36">600(-rw-------)</span> - Somente o proprietário tem acesso a gravar e ler o arquivo. Nenhum outro usuário pode ler, gravar ou executar o arquivo.
- <span style="color:#d97f36">777 (drwxrwxrwx)</span> - Não há restrições, qualquer um pode listar, adicionar ou excluir conteúdo do diretório
- <span style="color:#d97f36">755 (drwxr-xr-x)</span> - O dono do diretório tem todas as permissões, os outros usuários podem listar o diretório mas não podem criar arquivos nem excluí-los
- <span style="color:#d97f36">700 (drwx------)</span> - Somente o dono do diretório tem acesso total.