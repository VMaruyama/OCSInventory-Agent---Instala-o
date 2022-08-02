## Instalação OCS Inventory Agent

Para instalar um agente no próprio servidor basta seguir os procedimentos abaixo:
Instalação do pacote ocsinventory-agent:

<font color=\"red\">    **[root@ocs-inventory ~] # yum install -y ocsinventory-agent**</font>

Após instalação do pacote, é necessário alterar a indicação do servidor do OCS Inventory no arquivo de configuração do agente em /etc/ocsinventory/ocsinventory-agent.cfg. Onde as linhas correspondentes aos parâmetros server e local ficaram como:

Exemplo

<font color=\"red\">    **- server = http://192.168.1.1/ocsinventory**</font>

<font color=\"red\">**- #local = /var/lib/ocsinventory-agent**</font>

Para forçar que o agente envie os dados execute o binário do agente.

<font color=\"red\">**- ocs-inventory ~]# ocsinventory-agent**</font>

No painel foi necessário se desconectar e autenticar novamente (caso a sessão esteja aberta) para que as informações exibidas considerem o novo computador inventariado.

Pronto! Agora você já tem um OCS Inventory configurado e já sabe como instalar o agente.

.<font color=\"red\">Texto com cor vermelha</font>