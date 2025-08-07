 Wireshark: Basic Uses & Filters — Irfan’s Study Notes (Phase 1, Month 2)

Wireshark is a powerful packet analyzer used to capture and inspect network traffic in real-time. It’s essential for ethical hackers, red teamers, and network defenders alike.
 What Is Wireshark Used For?

    Capturing raw network packets in real time

    Analyzing protocol behavior (DNS, HTTP, TCP, etc.)

    Detecting misconfigurations, security flaws, and credentials in transit

    Performing deep inspection of suspicious or malicious traffic

 Basic Display Filters Learned
#	Filter	Description
1	dns	Displays only DNS traffic (queries and responses)
2	ip.addr == x.x.x.x	Shows all packets where the IP is either source or destination
3	ip.src == x.x.x.x	Only packets sent from the specified IP
4	ip.dst == x.x.x.x	Only packets received by the specified IP
5	tcp.port == 80	Displays only TCP packets on port 80 (HTTP)
6	udp.port == 53	Displays only DNS traffic on UDP port 53
7	http	Filters only HTTP protocol packets
8	icmp	Shows ICMP packets (like ping or traceroute)
9	tcp.flags.syn == 1	Displays TCP SYN packets (used to start TCP connections)
10	tcp.analysis.flags	Detects anomalies like retransmissions, dup ACKs, and broken sessions
11	frame contains "password"	Highlights packets containing the keyword "password"
12	tcp contains "user"	Same as above but scoped to TCP payloads only
 Mini Project: Sniffing HTTP Credentials

Goal: Demonstrate real-world packet analysis and credential capture over HTTP.
Setup:

    Launched a local test HTTP login server (no HTTPS)

    Entered sample login credentials (username: irfan, password: test123)

    Started Wireshark to capture traffic

Wireshark Filter Used:

frame contains "password"

Result:

    Successfully captured the HTTP POST request containing login credentials in plaintext

    Observed the password=test123 string directly in the packet payload

    Validated how insecure HTTP is for transmitting sensitive data

⚠Lesson:

    Never use HTTP for login forms. Passwords can be intercepted by anyone on the same network.
