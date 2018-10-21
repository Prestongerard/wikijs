<!-- TITLE: Journalctl -->
<!-- SUBTITLE: A quick summary of Journalctl -->

	# Check logs for iptable changes
	
	You can query the systemd journal for a "log" of the changes you made to the iptables service with:
	
$ journalctl -f -u iptables.service
$ journalctl -f -u ip6tables.service

found this in centos 7 tutorial