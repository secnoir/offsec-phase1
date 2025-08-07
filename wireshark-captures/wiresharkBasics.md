Wireshark basic uses and Filters i learned :
Wireshark is a network mapper 
1 : dns --> only shows packets related to DNS ( Domain Name System ) 
2 : ip.addr == x.x.x.x --> shows all packets where the IP adress is either the source of destination 
4 : ip.src == x.x.x.x	Only packets sent from that IP
5 : ip.dst == x.x.x.x	Only packets received by that IP
6 : tcp.port == 80	Shows only TCP traffic on port 80 (HTTP)
7 : udp.port == 53	Shows only DNS queries/responses
8 : http	Filters only HTTP protocol traffic
9 : dns	Filters only DNS protocol packets
10 : icmp	Shows ping/echo (Layer 3 diagnostics)
11 : tcp.flags.syn == 1	Shows only packets trying to start a TCP connection
12 : tcp.analysis.flags	Shows packets with TCP problems (retransmits, duplicate ACKs)
13 : frame contains "password"	Show packets containing the word "password" (can detect leaked creds)
14 : tcp contains "user"	Same idea, but focuses on TCP content only

SMALL PROJECT : used a test http server and put login and password then used wireshark Filter --> frame contains "password" to get the password


