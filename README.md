# zabbix-barman template

2nd Quadrant Barman monitoring template for Zabbix.

##Requirements:
In order to run this template there is needed to configure following options for Zabbix

1. Configure sudo option for zabbix user:
   `zabbix        ALL=(barman)      NOPASSWD: /usr/bin/barman`
2. Enable zabbix user shell access
   `usermod -s /bin/bash zabbix`
   
##Installation:
1. Put zabbix-barman-items.conf	on barman server
2. Restart zabbix-agent
3. Import zabbix-barman-template.xml

## General
There is auto discovery what will discover barman servers and items + triggers. 
