# Hash Cracker (Kali Linux)

## Overview
This project demonstrates the process of cracking password hashes using John the Ripper in a controlled lab environment. The aim was to understand how weak passwords can be identified through dictionary-based attacks.

---

## Tools Used
- Kali Linux
- John the Ripper
- rockyou.txt wordlist

---

## Steps Performed

mkdir -p ~/cyber-projects/hash-cracker

cd ~/cyber-projects/hash-cracker

echo -n "hello123" | md5sum

nano hash.txt

john --format=raw-md5 --wordlist=/usr/share/wordlists/rockyou.txt hash.txt

john --show --format=raw-md5 hash.txt

The original password "hello123" was successfully recovered from the hash using a dictionary attack.

## Key Learning

- Weak passwords can be easily cracked using dictionary attacks  
- Identifying the correct hash format is important  
- Wordlists significantly improve attack efficiency  
- Practical tools like John the Ripper are used in real-world security testing  
