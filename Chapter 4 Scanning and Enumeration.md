ping sweep uses ICMP (internet control message protocol)  packets o determine whether a hist is alive or not.

ICMP ECHO REQUEST (type 8) => ICMP ECHO REPLY (type 0)

# OSI Reference Model:
Physical => Bits
Data Link => Encapsulation and adding headers, MAC address and ARP => Frames
Network => IP => Packets
Transportation => TCP, UDP => Segments
Session => Data
Presentation => Data
Application => Data

# TCP/IP Reference Model:
Network Access
Internet
Transport
Application

# Well known port numbers (0-1023)
20/21 FTP => TCP
22 SSH => TCP
23 TELNET => TCP
25 SMTP => TCP (mail)
53 DNS => UDP for NS queries but TCP for zone transfers
67 DHCP => UDP
69 TFTP => UDP
80 HTTP => TCP
88 KERBEROS => both TCP and UDP

110 POP3 => TCP (mail)
135 RPC => TCP
137-139 NetBIOS => both TCP and UDP (microsoft windows)
143 IMAP => TCP (mail)
161/162 SNMP => UDP (simple network management protocol)
389 LDAP => both TCP and UDP  (jndi:ldap log4j exploit)
443 HTTPS => TCP
445 SMB => TCP (samba, wannacry, file share protocol)

TCP => connection-oriented protocol
UDP => connectionless protocol, fire packets are forget about them. => BROADCASTING

Three-way-handshake => SYN, SYN-ACK, ACK

Well known ports => 0-1023
Registered ports => 1024-49151
Dynamic ports => 49152-65535
Total # of ports => 2^16 = 65536

When we want to connect to google.com (HTTP), source port = 49245; destination port = 80

War dialing is the process where an attacker dials random phone numbers specifically looking a for a **network modem**.

War driving is the process where an attacker drives around in his car looking for openn access points.

Linux:
UID => user id
GID => group id

Windows:
SID => security identifier
RID = resource identifier

# Answers
B
A and C
C
D

C
C
D
A

A => B
D
D
A
