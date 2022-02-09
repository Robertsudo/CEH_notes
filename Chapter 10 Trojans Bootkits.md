Malware = malicious software

Trojan = a method to gain and maintain access to a machine (similar to backdoor)

Overt vs Covert communication channels => Open vs secret

HIDS (host IDS) and NIDS (network IDS) can detect trojan activity
Tripwire is an example of HIDS that can be used to verify the integrity of critical files.

# Virus types
Polymorphic/Metamorphic viruses change their own source code to avoid signature-based detection. The function of the code does not change.

Multipartite viruses attempt to infect **both** files and the boot sector at the same time.

A retrovirus is also referred to as an **anti-anti-virus** virus. This means that it tries to attack and disable any anti-virus or protective software on the system it is trying to infect to avoid detection.

------------------------------

Worms can be used to infect networks at once and then use them as bot-net zombies.

Sheepdip computers = Sandbox systems have AVs, port monitors, registry monitors, integrity checkers installed on them. (AV = AntiVirus)

Ping of death is **NOT**  a valid attack against modern systems. It is an old attack where an attacker sends a fragmented ICMP ping message and when the fragments are re-assembled on the target system the resultant ICMP packet is larger than the allocated buffer for it, so system crashes.

# Session Hijacking
1. Sniff the traffic
2. Monitor the traffic and predict the TCP/IP sequence numbering
3. Desynchronize the client's session using FIN or RST flags
4. Predict the session token and take over the session
5. Upon successful login, act as a real client.

*Sequence numbers are incremented (+1) upon acknowledgment. (SYN-ACK or ACK)

# Answers
D
C
A
C AND D

A AND C
B
C
D (Tripwire is NOT an AV. It is a file integrity checker.)

A
A