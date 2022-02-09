CGI = common gateway interface => handles request-response in web servers
ACL = access control list
SSI = server side includes (we can include/embed .docx .pdf kind of files inside an HTML page) (Most modern web browsers can open pdf files within the browser itself)
SSTI = server side template injection/inclusion

CGI scripts can run arbitrary commands on web server **with the permission of the web server user (NOT ROOT)**

Directory traversal = directory climbing = backtracking = dot dot slash attack => ../../../../etc/passwd 

# SQLi

SQL = structured query language
`anything' OR 1=1 --`

# XSS
`<img src=xxx:x onerror=javascript:alert(1)> -->`
`<script>alert(1)</script>`

# Buffer Overflows
Try to write more data into an application's pre-built buffer area in order to **overwrite** adjacent memory and then execute arbitrary code on that adjacent memory.
- Stack
- Heap
- NOP Sled (NOPS)(NO operation,909090...)

Protection against buffer overflows: => Use canary words to stop processing immediately when a canary word is altered. (halt the system)

# Answers
C
A
B=====> A (B is SQLi, A is parameter-tampering)
D

D
B
D
D

C
D