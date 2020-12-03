# zabbix-ambari

# Requisitos:
Zabbix versão >= 4.4

# Instruções de uso:
1) Instale o Template via import no zabbix;
2) Crie um HOST (não necessita de agent), associe o template ao HOST e modifique as MACROS do template junto ao seu host:
	{$AMB_URL} url do acesso do seu ambari;
	{$AMB_USER} usuário do ambari;
	{$AMB_USER} senha do ambari;
3) Configure os alertas no Ambari normalmente e sempre que um alerta aparecer no Ambari será exibido na console do Zabbix;

# Observações:
Todo alarme é identificado via regra de descoberta no zabbix em chamada HTTP API do Ambari.


Version

    1.0 - initial