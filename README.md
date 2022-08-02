## Instalação OCS Inventory Agent

Para instalar um agente no próprio servidor basta seguir os procedimentos abaixo:
Instalação do pacote ocsinventory-agent:

**[root@ocs-inventory ~] # yum install -y ocsinventory-agent**

Após instalação do pacote, é necessário alterar a indicação do servidor do OCS Inventory no arquivo de configuração do agente em /etc/ocsinventory/ocsinventory-agent.cfg. Onde as linhas correspondentes aos parâmetros server e local ficaram como:

Exemplo

**- server = http://192.168.1.1/ocsinventory**

**- #local = /var/lib/ocsinventory-agent**

Para forçar que o agente envie os dados execute o binário do agente.

**- ocs-inventory ~]# ocsinventory-agent**

No painel foi necessário se desconectar e autenticar novamente (caso a sessão esteja aberta) para que as informações exibidas considerem o novo computador inventariado.

Pronto! Agora você já tem um OCS Inventory configurado e já sabe como instalar o agente.