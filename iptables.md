<!-- TITLE: Iptables -->
<!-- SUBTITLE: A quick summary of Iptables -->

# Command rules
sudo iptables -p tcp -A INPUT --dport 22 -m state --state NEW,ESTABLISHED -j ACCEPT
sudo iptables -p tcp -A OUTPUT --sport 22 -m state --state ESTABLISHED -j ACCEPT
sudo iptables-save > /etc/iptables/rules.v4