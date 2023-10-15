# Sample Exam

This sample exam set is roughly half the size of a normal ITS exam.

## A. Short answer questions

1. Briefly explain the security principle of least privilege.

2. A block cipher requires a mode of operation, why?

3. How does a worm differ from a virus?

4. Is a TLS connection to your bank secure even if their web server has a buffer overflow vulnerability?

5. Does placing a firewall in front a website protect against SQL injection attacks?

6. Are signature-based intrusion detection systems good at identifying novel network attacks that have not been previously seen?

## B. Security Principles

1. Some people lock valuables in a safe in their house in addition to locking the doors of the house. Which security principle is being followed here?

2. Some people place an extra key to their house under one particular stone in the front yard in case they forget or lose their main key. Which security principle is being followed here?

3. Some people will, even though they have a safe, hide important documents in between pages of a book in their living room. Which security principle is being followed here?

## C. Password Storage

You are tasked to review and advise how to securely store users' password in a database used by a new website being developed.

Review below independent password storage schemes. In all cases, assume an attacker has access to the entire database. Also assume that there are n users who each choose from a common pool of n possible passwords, i.e the attacker knows all possible cleartext passwords, and the attacker has enough compute power to perform O(n) hashes, decryptions, XORs, and other computations.

In this question, H is a secure cryptographic hash function, ⊕ denotes bitwise XOR, and || denotes concatenation.

1. For each user, the database stores (username, H(password)). Which of the following statements are true? Select all that apply.
a The attacker can determine all pairs of users who share the same password.
b The attacker can learn all users’ passwords.
c The attacker can learn at least one user’s password.
d None of the above

2. For each user, the database stores (username, h(username) ⊕ password). Which of the following statements are true? Select all that apply.
a The attacker can determine all pairs of users who share the same password.
b The attacker can learn all users’ passwords.
c The attacker can learn at least one user’s password.
d None of the above

3. For each user, the database stores (username, s, H(password || s)) where s is a random 1024-bit value. Which of the following statements are true? Select all that apply.
a The attacker can determine all pairs of users who share the same password.
b The attacker can learn all users’ passwords.
c The attacker can learn at least one user’s password.
d None of the above

## D. Network Security

1. Explain the difference between packet filters and web application firewalls.

2. How effective is a firewall at:
- Preventing port scanning.
- Preventing malware downloads by internal users.
- Preventing malware on internal users' workstations to communicate outbound.

3. You have made a network trafic recording, a PCAP file, of malware communicating to a previously unknown bad domain. Would you expect a NIDS like Snort to able to detect it? Why or why not?

## E. TLS

1. Briefly explain the use of RSA in TLS.

2. Suppose an attaker steals the private RSA key of a server that uses TLS. What can an attacker do with the key?

3. Suppose another server is configured to use Diffie-Hellman only for key exchange when TLS sessions are set up. How is this less or more secure than relying RSA in TLS?

4. In TLS, we verify the identity of the server, but not always the client. How can clients be verified?


