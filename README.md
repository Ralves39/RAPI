# RAPI
RAPi uma nova visão para zabbix (Compativel com a versão 4.0 +)
Criado para ser um dashboard automatizado e simplificado para zabbix. não requer instalação adicional apenas um apache e php que são nativos do zabbix (ideal para ser instalado na mesma maquina do front end do zabbix)

1 - realize o download do arquivo zip e descompacte na sua pasta padrão do apache (exemplo /var/www/html)
2 - apos edite o arquivo de configuração encontrado na pasta /var/www/html/rapi/conf/conf.php inserindoos seguintes dados
//Configuração de acesso ao front End zabbix-API

$user_zbx='Admin'; <--------- Usuario com acesso a API do zabbix

$passwd='zabbix'; <---------- Senha do usuario

$ip_zbx='localhost'; <---- ip do zabbix server

Funcionalidade
* Dashboard com alarmes e severidade
* painel retratil de alarmes com suas descrições e grupos do host
* função de reconhecimento do evento incluindo menssagem de sinalização
* somatorio de alarmes ativos no ambiente separado por grupo
* indicação de alarmes onde o host esta em manutenção.

Observação e Dicas: 
1 - refresh time da pagina - O tempo de refresh do painel é de 30 segundos, caso queira um tempo maior ou menor insira a variavel refresh na URL em formato php e o tempo sendo indicado em segundos. Exemplo
Refresh da pagina em um tempo de 10 minutos
http://192.168.1.169/rapi/dashboard.php?refresh=600

2 - Ambientes com varios alarmes - em ambientes com grande quantidade de alarmes ou manutenções em hosts, considere separa o frontend do zabbix para uma resposta rapida da API. Como este dashboard consulta totalmente a API, considere deixa-lo o mais rapido possivel nestes ambientes.


Objetivo do projeto - desenvolver um dashboard automatico e dinâmico que ajude nas funções do dia dia, para as pessoas não familiarizadas com as telas do zabbix, e que proporcione o minimo nescessário para administração dos eventos do dia-dia. Alem de ajudar no aprendizado da ferramenta e suas consultas via sua poderosa API. 

Espero que gostem e divirtam-se em seus desenvolvimentos com a ferramenta. Lembrando que se gostar não deixe de comentar e de compartilhar, para que eu possa ter mais oportunidades no mundo Zabbix.

English Version

RAPi a new vision for zabbix (Compatible with version 4.0 +)
Designed to be an automated and simplified dashboard for zabbix. no additional installation required just an apache and php that are native to zabbix (ideal to be installed on the same machine as zabbix front end)

1 - Download the zip file and unzip your default apache folder (example / var / www / html)
2 - Bet the configuration file found in the /var/www/html/rapi/conf/conf.php folder by entering the following data
// Configuring zabbix-API Front End Access

$ user_zbx = 'Admin'; <--------- User with zabbix API access

$ passwd = 'zabbix'; <---------- User Password

$ ip_zbx = 'localhost'; <---- zabbix ip server


Functionality
* Panel with alarms and severity
* retractable alarm panel with their descriptions and host groups
* event recognition function including signaling measurement
* sum of active alarms in group-separated environment
* indication of alarms where the host is under maintenance.

Note and Tips:
1 - page refresh time - The panel refresh time is 30 seconds, if longer or shorter, between a variable URL update in php format and the time being indicated in seconds. Example
Refresh page within 10 minutes
http://192.168.1.169/rapi/dashboard.php?refresh=600

2 - Multi-Alarm Environments - In high-alarm or host-maintenance environments, consider zabbix splitting or frontend for a quick API response. Since this panel fully queries an API, consider leaving it as soon as possible in these environments.


Project Objective - To develop an automated, dynamic dashboard that will help with day functions for people unfamiliar with zabbix displays and provide the minimum necessary to manage day events. In addition to helping you learn tools and queries through the powerful API.
I hope you enjoy and have fun in your developments with the tool. Remembering that if you like be sure to comment and share, so I can have more opportunities in the Zabbix world.

Rodrigo Soares
rodrigo_s.alves@hotmail.com
Linkedin - https://www.linkedin.com/in/rodrigo-soares-alves-7312733b/
