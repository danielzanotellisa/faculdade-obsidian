#Conceitos_de_redes 
#Servidores 
# Oque é

---

O FTP oferece a capacidade de transferir arquivos entre um cliente e um servidor. Um cliente FTP é um aplicativo que serve para enviar e receber arquivos de um servidor que executa FTP como um serviço. Para transferir dados com sucesso, o FTP precisa de duas conexões

 1. Conexão de controle: Conexão que o cliente abre para controlar o tráfego
 2. Conexão de dados: O cliente abre a segunda conexão para o tráfego de dados

O FTP tem deficiências na segurança, por isso devem ser usados outros serviços para transferência de dados.

- FTPS: Faz com que o protocolo FTP seja criptografado, o servidor pode aceitar ou não a requisição
- SSH File Transfer Protocol (SFTP): Extensão do SSH, usado para estabelecer uma sessão segura de transferência de arquivos
- SCP(Secure Copy Protocol): Também usa o SSH para proteger os arquivos