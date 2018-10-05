<!-- TITLE: Du -->
<!-- SUBTITLE: A quick summary of Du -->

# Displays 5 largest log files and size

$ cd /var/log
$ sudo du * | sort -nr | awk 'BEGIN {OFMT = "%.0f"} {print $1/1024,"MB", $2}' | head -5