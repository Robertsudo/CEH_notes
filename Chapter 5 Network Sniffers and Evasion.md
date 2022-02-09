Sniffer, to sniff (v) by nose

## Examples of Sniffers
Wireshark
Ettercap
EtherPeek
Snort (also an IDS)
tcpdump (unix) OR windump (linux) => command line only, no GUI
Winsniffer

## ARP spoofing, poisoning
Cain and Abel
dsniff
SMAC

# IDS = intrusion detection systems
Signature-based vs anomaly-based

SNORT ! => most widely used IDS in the world
can detect port scans, OS fingerprinting attempts, buffer overflows ..

Snort config files stay in:
/etc/snort
C:\snort\etc

Snort rules: => /etc/snort/rules

`var HOME_NET 192.168.1.0/24
alert tcp !$HOME_NET any -> $HOME_NET 23 content "admin" (msg: "Telnet attempt with admin access"`

# IDS Evasion
1. Encryption, if there is no SSL-stripper put in place, IDS normally cant read encrypted data: SSH-HTTPS
2. Being stealth. NMAP T5 scan can be detected immediately whereas slow T1 scan may slip undetected.
3. Cover-fire: If we have a list of IP-addresses to sacrifice, we can use them to port scan. They will eventually get blacklisted though.
4. Insider access. Using a compromised machine as C2-agent.

# Private Network Classes (NOT ROUTABLE)
192.168.0.0
172.16-31.0.0
10.0.0.0

Firewalking:  "Walking" through every port against a firewall to determine what ports are open

# Answers
D
B AND C
D
B => C

A
C
B
A => B (ARP poisoning must be done on the sender machine. NOT on the router)

C
D AND B
D AND A ====> C AND A