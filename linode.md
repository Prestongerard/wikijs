<!-- TITLE: Linode -->
<!-- SUBTITLE: A quick summary of Linode -->

# Common commands for tix

$ sudo iptables-save 

$ sudo netstat -plntu
——————————
sudo mtr -P 22 -i 0.5 -rwc 50 172.104.173.70

———————————

time curl -v --trace-time http://www.cloudcapsule.cc/test2.php

This command will let us know whether slowness is network, server, or website based.
_________________________

egrep -i '(password|permit|port|rsa)' /etc/ssh/sshd_config

What the above command does is pull out any line in your sshd_config file that contains the following words: password, permit, port and rsa. 
____________________________

sudo iptables -p tcp -A INPUT --dport 22 -m state --state NEW,ESTABLISHED -j ACCEPT
sudo iptables -p tcp -A OUTPUT --sport 22 -m state --state ESTABLISHED -j ACCEPT
sudo iptables-save > /etc/iptables/rules.v4

_____________________________________________________________________________

sudo ss -plant4
ip a | grep eth0
sudo service mysql status
sudo service apache2 status
iptables -L
