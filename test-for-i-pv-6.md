<!-- TITLE: Test For I Pv 6 -->
<!-- SUBTITLE: A quick summary of Test For I Pv 6 -->

# Test
$ dig A example.com +short
$ dig AAAA example.com +short

if you get an IPv6 address, then check it with curl.

$ curl -4 -sIL example.com
$ curl -6 -sIL example.com

I bet the -4 gets a response and the -6 doesn't.

find out what web server they are using then:
1. update virtualhost (apache) or server listen directive (nginx) to support ipv6.
or
2. remove the AAAA record.