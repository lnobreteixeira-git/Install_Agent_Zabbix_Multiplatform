# Install_Agent_Zabbix

  - Autores: Clayton Teixeira e Lucas Nobre Teixeira
  
  Objetivo: instalação de agente Zabbix multiplataforma abrangendo dos seguintes sistemas operacionais:
  . Linux (Debian , ubuntu, xubuntu, lubuntu ...)
  . Linux (CentOS, Fedora, RedHat ...)
  . AIX (7.x)
  . Windows (7, 8, 10 , 11 ...)
  
# Instalação:
  
  A automação da instalação dos agentes do Zabbix multiplataforma é feita através do ANSIBLE, portanto é imprescindível ter o Ansible instalado e operacional.
  Uma vez que você já tem o Ansible instalado baixe este git no /etc/ansible (raiz do ansible).
  Observação importante: Seria excelente se o servidor ansible tiver troca de chave SSH entre os hosts descritos no arquivo de inventário do ansible (aqui arquivo hosts)
  
  
# Configurar:
   a) Edite o arquivo hosts (inventário) criando grupos entre colchetes [] exemplo:  [LINUX]
   b) Abaixo da tag de grupo exemplo [LINUX], coloque a lista de servidores linux um em cada linha se seu computador resolve nomes via DNS local pode ser o hostname caso contrário o endereço IP.
   c) Edite o arquivo ansible.cfg se achar conveniente, ele já está preparado para comunicação com Linux, AIX e Linux.
   
