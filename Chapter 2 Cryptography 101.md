function(plaintext) => yield(ciphertext)

How do we encrypt bits?
1. By substitution => bits are replaced by other bits.Replace "A" with "B" (Caeser Cipher), "BABA" => "ABAB"
2. By transposition => the order of bits is changed. "BABA" => "AABB"

# Block Ciphers vs Stream Ciphers
In stream ciphers, bits of data are encrypted as a continuous stream.  Every bit is encrypted one at a time, usually by an XOR (exclusive-OR operator).
However if the key length used is smaller than the actual data, the stream cipher will be vulnerable to frequency attacks.
Example: data => 101010
key => 111
result => 010101

In block ciphers, bits of data are divided into small blocks and then encrypted using substitution and transposition.

# Symmetric vs Asymmetric Encryption
Symmetric => single shared key is used both to encrypt and decrypt the data.
Asymmmetric => two keys, public key vs private key.
Public key can be sent to everyone freely (Newsletter reporters share their public key on twitter)
Public key can generally be used for encryption.
Private key can generally be used for decryption.
Exception: Private key can also be used for encryption when we want to sign a message (Digital signature)

Symmetric => DES, AES, Blowfish
Asymmetric => RSA, Diffie-Helman, Elliptic Curves (Public and Private Keys)

# Hashing
One-way hashing algorithms do not encrypt anything at all.
The only purpose of hashing is to verify the **integrity** of a data.

Example hash functions => MD5, SHA-1,2,3 (by NSA)

Password hashes must be protected with salts. Every bit of salt increases the complexity by a factor of 2.

Even though hashes are one-way functions, we can use **collision attacks** and rainbow tables (hash-value tables) to "crack" easy passwords.

Any deviation (change, alteration) in hash value indicates corruption. Re-install needed.

# PKI = Public Key Infrastructure
CA = Certificate Authority
RA = Registration Authority

Encryption provides confidentiality.
Hashing provides integrity.
Plaintext = cleartext
Ciphertext = encrypted, unreadable text

Non-repudiation = The sender **cannot** deny he sent the message **AND** the receiver **cannot** deny he received the message. NON-DENIABILITY (legal term)

# Answers
B
B
C
B

D
C ====> D
A
D

C
D
C
C
D =====> A
