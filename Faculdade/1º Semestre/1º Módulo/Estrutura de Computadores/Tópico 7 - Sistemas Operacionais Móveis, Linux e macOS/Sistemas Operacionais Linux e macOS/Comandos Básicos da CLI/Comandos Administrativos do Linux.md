#EstruturaDeComputadores #SIstemaOperacional #Linux 


# Comandos
---

### <span style="color:#d97f36">passwd</span>
- Permite que usuários alteram sua própria senha no terminal
- É necessário saber a senha atual
- Por motivos de segurança, nem os caracteres nem um asterisco são exibidos durante a digitação
- ![](../../img/Pasted%20image%2020240325135808.png)

### <span style="color:#d97f36">ps</span> 
- Permite que os usuários monitorem seus próprios processos
- Sem especificar opções, o comando ps mostra apenas os usuários dos programas em execução no terminal atual
- ![](../../img/Pasted%20image%2020240325135924.png)
- O segundo comando ps usa a opção <span style="color:#d97f36">-e</span> indicando tudo. A saída do comando é canalizada para o comando grep para procurar linhas de saída que correspondam à palavra gnome.
### <span style="color:#d97f36">kill</span> 
- Permite que os usuários finalizem os processos iniciados
- Man Kill para exibir as opções úteis para o comando Kill
- ![](../../img/Pasted%20image%2020240325140121.png)

### <span style="color:#d97f36">ifconfig</span> 
- Usado quase da mesma forma que o comando Windows ipconfig
- Esse comando é preterido e o comando "<span style="color:#d97f36">endereçoIP</span>" deve ser usado em vez disso
- ![](../../img/Pasted%20image%2020240325140306.png)

### <span style="color:#d97f36">iwconfig</span> 
- Um dos muitos comandos sem fio que começam com as letras "<span style="color:#d97f36">IW</span>"
- Permite que os usuários definam e visualizem suas configurações sem fio
- ![](../../img/Pasted%20image%2020240325140353.png)

### <span style="color:#d97f36">chmod</span> 
- Comando que permite que os usuários alteram suas permissões dos próprios arquivos
- ![](../../img/Pasted%20image%2020240325140445.png)

## Comandos que exigem acesso à raiz(root)
---

### <span style="color:#d97f36">sudo</span> 
- Concede um acesso à raiz do usuário sem alterar realmente o perfil
- Acesso concedido por tempo limitado
- Apenas se o usuário estiver listado no arquivo /etc/sudoers
- ![](../../img/Pasted%20image%2020240325140645.png)

### <span style="color:#d97f36">chown</span> 
- Permite que os usuários alterem o proprietário e o grupo de um ou mais arquivos
- usar esse chown -r rever todos os arquivos no diretório base de um usuário para eles
- ![](../../img/Pasted%20image%2020240325141013.png)

### <span style="color:#d97f36">apt-get</span> 
- Usado para instalar e gerenciar o software em distribuições Linux com base em Debian
- Podemos usar somente "apt"
- ![](../../img/Pasted%20image%2020240325141143.png)

### <span style="color:#d97f36">shutdown</span> 
- Usado para interromper e reinicializar o SO
- Possui recursos para avisar os usuários sobre um desligamento iminente e agendar um desligamento no futuro
- ![](../../img/Pasted%20image%2020240325141426.png)

### <span style="color:#d97f36">dd</span> 
- Usado para copiar arquivos e partições e criar arquivos de troca temporários
- Deve ser usado com extrema cautela
- ![](../../img/Pasted%20image%2020240325141525.png)
