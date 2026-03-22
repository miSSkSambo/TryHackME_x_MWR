# 🔐 Encoding, Encryption & Hashing 

---

## 🎯 What This Assignment Is About

This assignment focuses on three fundamental cybersecurity concepts:

🔄 **Encoding** – Converting data into a different format for transmission (e.g., Base64, URL Encoding). It is reversible and not meant for security.  

🔐 **Encryption** – Protecting data by converting it into ciphertext using a key so that only authorized users can access it.  

#️⃣ **Hashing** – A one-way process used to protect data like passwords. It cannot be reversed and is used for verification and integrity.  

---

### 💡 What You Learn

- How data is transformed and transmitted across systems  
- How encryption secures sensitive information  
- How hashing protects passwords and data integrity  
- How attackers crack hashes using tools like Hashcat  
- Why poor implementations lead to vulnerabilities  

👉 This assignment builds the foundation for:
- Web security  
- Ethical hacking  
- Penetration testing  
- Secure application development  

link to the room: https://tryhackme.com/jr/mwr-virtual-internship-week-2-we-love-cybersec  
---
## task 1[introduction]
completed

---

## task 2[encoding]

Q: What Encoding Schema is also called percent encoding?
A: URL Encoding

Q: Decode TXkgRmlyc3QgQmFzZTY0IERlY29kZQo=
A: My First Base64 Decode

Q: What HTML characters should be encoded to prevent XSS
A: &,<,>,",'

Q: Please URL Decode Key Characters for:
%2Froom%2Fmwr-virtual-internship-week-2-we-love-cybersec%3FParameter%3DURL%20parameter%201%26Param2%3DAnother%20we!rd%20parameter
A: /room/mwr-virtual-internship-week-2-we-love-cybersec?Parameter=URL parameter 1&Param2=Another we!rd parameter

Q: What is the HTML encoded value for &
A: &amp

---

## task 3[encryption]

Q: What do you call the encrypted plaintext?
A: ciphertext

Q: Can you encrypt the following with Triple DES.
Value = "Let's encrypt something", key = "Weneeda24bytekeyforthis1, IV = "Theivis8"
A: d1cd629d1771610b41b2d4975acc178f3d158b4fd66cf5bf

Q: Can you decrypt the following data. Encryption schema is "Blowfish".
mode = "CBC", key = "Thisisakey", IV = "password", Encrypted value = "88f022072f8c065c8abd87b19b35008b6c9763b78a9e4834"
A: MWR{Encryption-is-Fun}

Q: Challenge: This one will use a couple schemas, can you get the original text? The original encryption process was
1. To MorseCode
2. Vigenère Encode - key = "Password"
3. CipherSaber2 Encrypt - key = "secret" - 20 rounds
4 To Base62

ZeDVewLvGNZDRKb5Xsr2VzZA6tz81KxO7QkXkxoNgO3ZadhRXqTYh8YooemW5rRGNhRyapE2RxVUTo
A: You got the flag

---

## task 4[historical ciphers]

Q: Knowing that XRPCTCRGNEI was encrypted using Caesar Cipher, what is the original plaintext?
A: ICANENCRYPT

---

## task 5[hashing]

Q: What is the output size in bytes of the MD5 hash function?
A: 16

Q: Can you avoid hash collisions? (Yea/Nay)
A: Nay

Q: Should you encrypt passwords? Yea/Nay
A: Nay

Q: Crack the hash "5f4dcc3b5aa765d61d8327deb882cf99"
A: password

Q: Crack the hash "dc647eb65e6711e155375218212b3964"
A: Password

Q: What hashing format is this hash 'e22084c2ca255918f9f9c755e06e9dbe7cdf13f0635bdcafaa6dbc8ba963c25b'
A: sha256

Q: Can I get the input of the hash, from the output? (yay/nay)
A: nay

---

## task 6[cracking hashes]

Q: Crack this hash: $2a$06$7yoU3Ng8dHTXphAg913cyO6Bjs3K5lBnwq5FJyA6d01pMSrddr1ZG
A: 85208520

Q: Crack this hash: e24df70c9d9c81d60f0e475be740a6cee28744087976f74974d4390396ce36f1
A: sadierose

Q: Hash: Hash: faa2b8b7cd11d908f101df15a0b12d4c05a89abc9604df0f275a4fc9a00280027c95c4b0e1dfa314b2c4224e820146568205ffd1e58eb7bf6fd07dfe79b83060
A: class1999

Q: Crack this hash: 978d75c9de6daf87868795326184dc76e0c4dd0e33e53b0d7a988b180d90ef65
A: n63umy8lkf4i

Q: Hash: e5d8870e5bdd26602cab8dbe07a942c8669e56d6
- Salt: tryhackme
A: 481616481616
