ipstats
=======

Command line tool to display ipv4/ipv6 throughput stats on OSX and Linux on the console
Where possible it displays separate stats for IPv4 and IPv6.
Testing shows it reports more accurate speeds than speedtest.net or similar web based speed test sites

Linux support is more limited due to less stats available in netstat, I had to use iptables to get any IPv4/IPv6 data.
Improvements/contibutions are welcome.

Example output:

$ ipstats
TIME				  en1 In / Out Mbps	IPv4 packets	IPv6 packets	TCP Mbps	TCPv4 In / Out Mbps	TCPv6 In / Out Mbps
Tue  4 Feb 2014 22:53:25 GMT :: en1 : 0.01 / 0.01	IPv4 : 1	IPv6 : 24	TCP : 0.00	TCPv4 : 0.00 / 0.00 	TCPv6 : 0.00 / 0.01
Tue  4 Feb 2014 22:53:30 GMT :: en1 : 0.03 / 0.03	IPv4 : 2	IPv6 : 42	TCP : 0.03	TCPv4 : 0.00 / 0.00 	TCPv6 : 0.03 / 0.02
Tue  4 Feb 2014 22:53:35 GMT :: en1 : 16.94 / 0.42	IPv4 : 3	IPv6 : 7297	TCP : 15.52	TCPv4 : 0.00 / 0.00 	TCPv6 : 16.89 / 0.18
Tue  4 Feb 2014 22:53:40 GMT :: en1 : 45.38 / 0.43	IPv4 : 3	IPv6 : 18921	TCP : 42.88	TCPv4 : 0.00 / 0.00 	TCPv6 : 43.88 / 0.17
Tue  4 Feb 2014 22:53:45 GMT :: en1 : 46.44 / 0.40	IPv4 : 11	IPv6 : 19370	TCP : 43.89	TCPv4 : 0.01 / 0.00 	TCPv6 : 44.89 / 0.16
Tue  4 Feb 2014 22:53:50 GMT :: en1 : 24.30 / 0.21	IPv4 : 0	IPv6 : 9962	TCP : 22.37	TCPv4 : 0.00 / 0.00 	TCPv6 : 22.58 / 0.08
Tue  4 Feb 2014 22:53:55 GMT :: en1 : 2.03 / 0.01	IPv4 : 2	IPv6 : 850	TCP : 1.92	TCPv4 : 0.00 / 0.00     TCPv6 : 1.96 / 0.00
