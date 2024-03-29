#AmeaçaASegurança #EstruturaDeComputadores #Segurança #Rede 



- Tipos comuns de alvos em um ataque a rede
	- Executar consulta de informações de um alvo
	- Varredura de ping da rede de destino para determinar quais endereços IP estão ativos
	- Verificação de porta nos endereços IP ativos
	- Scanners de vulnerabilidade
	- Ferramentas de exploração
- Ataques TCP/IP
	- Negação de serviço (DoS)
		- Sobrecarrega completamente um dispositivo de destino com solicitações falsas para criar uma negação de serviço para usuários legítimos
		- Desconectar um dispositivo essencial para causar falhas na rede
	- DoS Distribuída (DDoS)
		- Usa muitos hosts infectados, denominados "zumbis" para sobrecarregar um alvo
		- Usam um computador manipulador para controlar um exército de hosts comprometidos
		- Botnets permanecem inativos até que sejam instruídos pelo manipulador
			- Podem ser usados em SPAM e phising
	- Envenenamento de DNS
		- Registros de DNS falsos redirecionam para servidores mal intencionados
	- Man in the Middle 
		- Intercepta a comunicação entre dois hosts
		- Pode capturar pacotes e visualizar o conteúdo, manipular e muito mais
		- Podem ser criados usando um ataque de spoofing de ARP
	- Replay
		- Uma repetição de um ataque de falsificação
			- Capturou um pacote autenticado
			- Alterou o conteúdo
			- Enviou para o destino original
		- O host de destino aceita o pacote alterado como autêntico
	- Spoofing
		- Falsifica os endereços IP para obter acesso aos recursos
	- Inundação de SYN
		- Tipo um DDoS que explora o handshake triplo do TCP
		- Envia solicitações de SYN falsas contínuas ao destino
		- O destino é sobrecarregado e não é possível estabelecer solicitações de SYN válidas, criando um ataque DoS