---
title: Encryption
description: Introduction to encryption concepts and techniques.
hideInToc: false
background: https://cover.sli.dev
layout: cover
transition: fade
---

# Encryption

## From the Study Design:

applications of cryptographic techniques to protect data at rest and in transit, including:
- use of ciphers
- symmetric and asymmetric keys
- use of hashing functions

---
layout: center
zoom: 0.6
---

# Introductory Video

<SlidevVideo controls>
  <!-- Anything that can go in an HTML video element. -->
  <source src="/video/secrets.mp4" type="video/mp4" />
  
  <p>
    Your browser does not support videos. You may download it
    <a href="/video/secrets.mp4">here</a>.
  </p>
</SlidevVideo>

Video generated using NotebookLM - [https://notebooklm.google.com/](https://notebooklm.google.com/)

---
layout: two-cols
zoom: 1.2
---

# Encryption At Rest

- Data that is stored on a device or server
- Protects data from unauthorized access if the device is accessed, lost or stolen
- Examples: Full disk encryption, database encryption, file-level encryption

::right::

# Encryption In Transit

- Data that is being transmitted over a network
- Protects data from interception or eavesdropping during transmission
- Examples: HTTPS, VPNs, TLS/SSL

---
layout: two-cols
zoom: 1.1
---

# Ciphers

A method of transforming readable data (plaintext) into an unreadable format (ciphertext) using an algorithm and a key.

- **Substitution Ciphers**: Replace each letter with another letter (e.g., Caesar cipher)
- **Modern Ciphers**: Use complex algorithms and keys (e.g., AES, DES)

**Ciphers allow for data to be decrypted back to its original form using the appropriate key.**

::right::

# Hashing Functions

A one-way function that transforms data into a fixed-size string of characters, which is typically a sequence of numbers and letters.
- Common hashing algorithms: MD5, SHA-1, SHA-256
- Used for data integrity verification and password storage

**Hashing is not reversible; original data cannot be retrieved from the hash.**

---
layout: two-cols
zoom: 1.1
---

# Symmetric Key Encryption

- Same key is used for both encryption and decryption
- Faster and more efficient for large amounts of data
- Key must be kept secret and shared securely
- *Examples: AES, DES, 3DES*

::right::

# Asymmetric Key Encryption

- Uses a pair of keys: a public key for encryption and a private key for decryption
- More secure for key distribution, but slower than symmetric encryption
- Commonly used for secure communications (e.g., SSL/TLS)

- *Examples: RSA, ECC*

---
layout: cover
zoom: 1
---

# Summary
- Encryption protects data at rest and in transit
- Ciphers transform data between plaintext and ciphertext
- Symmetric encryption uses the same key for both encryption and decryption
- Asymmetric encryption uses a pair of keys for secure communication
- Hashing functions provide data integrity verification but are not reversible

---
layout: center
---

# Do Now: Questions

1. What type of encryption helps to verify the integrity of data that has been transmitted?
2. Which type of encryption uses a public and private key pair?
3. What is the main difference between encryption and hashing?
4. Name one example of a symmetric encryption algorithm.
5. Explain why a system might use hashing to protect passwords?

---
layout: center
zoom: 0.8
hideInToc: false
visible: false
---

# SAC Marking Notes

<v-clicks>

- **Data Integrity:** quote the characteristics of data integrity
- **Password Policies:** changing passwords every 60 days is actually pretty good. More often than that and people use other less secure ways to remember them.
- **"Evaluate and explain"** - tripped lots of you up. Lots did one but not the other.
- **Check any numbers** - e.g "two strategies" - make sure you clearly talk about two different strategies.
- Question 6 (Describe how issues with the current strategy contributed to the data breach) - **answered really well!** 
- **Know your laws** - Privacy Act, Privacy and Data Protection Act, Health Records Act, Notifiable Data Breach Amendment
- **Threats** - Accidental, Deliberate, Event-based. Then describe them. Not the characteristics of data integrity.
- Question 9 - "Evaluate how... impact on integrity" - Lots of blanks. **Characteristics of data integrity again.**
- 
</v-clicks>

---