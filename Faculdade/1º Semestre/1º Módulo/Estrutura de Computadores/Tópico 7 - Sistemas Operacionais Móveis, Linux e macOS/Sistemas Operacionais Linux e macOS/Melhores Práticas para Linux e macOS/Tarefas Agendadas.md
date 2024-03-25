#EstruturaDeComputadores #SIstemaOperacional #Linux #macOS 



# Oque são
---

- Tarefas de manutenção preventiva que podem ser programadas para ocorrerem de tempos em tempos pelo SO
- Tarefas como backups e verificações de disco podem ser agendadas e executadas automaticamente.
- Um benefício das tarefas agendadas é que elas possibilitam que o computador realize essas tarefas quando nenhum usuário estiver utilizando o sistema.
- O utilitário CLI "<span style="color:#d97f36">cron</span>" pode agendar essas tarefas fora do horário de pico
- O <span style="color:#d97f36">cron</span> usa uma tabela de agendamento que pode ser editada com o comando crontab
	- ![](../../img/Pasted%20image%2020240325115419.png)
	- A tabela cron é um arquivo de texto sem formatação que possui seis colunas
	- Uma tarefa é representada por um comando, um programa ou um script
	- Para agendar uma tarefa, o usuário adiciona uma linha na <span style="color:#d97f36">crontab</span>
	- Quando a data e a hora especificadas chegam, a tarefa é executada.
	- ![](../../img/Pasted%20image%2020240325115638.png)
	- ![](../../img/Pasted%20image%2020240325115705.png)
	- Para criar uma <span style="color:#d97f36">crontab</span>, utilizamos o comando <span style="color:#d97f36">crontab -e</span> em um terminal
	- Para listar a <span style="color:#d97f36">crontab</span> atual, usamos o comando <span style="color:#d97f36">crontab -l</span> 
	- Para remover a <span style="color:#d97f36">crontab</span>, utilizamos o comando <span style="color:#d97f36">crontab -r</span> 
