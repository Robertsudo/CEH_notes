# Password attacks
Passive online attack => Man-in-the-middle (MITM) or re-play (at-a later time) attacks
Cain and Abel (tool) can sniff network traffic and capture id/passwd info in cleartext protocols (FTP,telnet,HTTP)

Rainbow tables = huge files of hashes-cleartexts for comparison.

# where passwords are stored?
/etc/passwd AND /etc/shadow
C:\Windows\System 32\Config\SAM

Gaining access => **Escalating Privileges** => Maintaining Access

## Microsoft Windows Technologies
NT = New technology
NTFS = New technology file systme
NTLM = New technology LAN manager (for passwords)(LAN = local area network)

Alternate Data Streams (ADS) in the form of NTFS file streaming
Example:
`type I_want_to_hide_this.txt > Public.txt:hidden`
This command **appends** argv1 to argv2 in a hidden way. Not listable when using "dir" or "ls".

changing attributes from normal to hidden:
`attrib +h filename` (or -h)

A rootkit is designed to obscure system compromise.

# 3 Types of Rootkits
1. Application level => Replace legitimate app. files with trojan binaries
2. Kernel level => executes at negative rings or even on the boot sector. persistent. NSA level
4. Library level => use syscalls to hide existentence

# Linux

Windows root directory (path) => C:\ wheras Linux root path => /
C:\Windows\System32 <=> /bin (executable binaries)

LKM = linux kernel module
to load them: `modprobe LKM_name`
# Review
1. Passive online password attacks => Sniffing a wire, sniffing network traffic
2. Sidejacking => Stealing cookies and then replaying them
3. Active online password attacks => Simply guessing on login form
4. Offline password attacks => pulling /etc/passwd and /etc/shadow and working on them on a separate machine. dictionary attacks, brute-force

# Answers
D ============> C (ADS in NTFS)
A
B
B => C ==============> A (most guaranteed way)

C
C
A and B and C
B

D
A
B
C
