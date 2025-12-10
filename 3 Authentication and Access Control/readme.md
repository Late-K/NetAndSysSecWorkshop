# LAB 3

Networks and Systems Security
Week 03
Authentication and Access Control

## Aims of the Seminar

In this workshop, we'll
dive into the essential principles of modern authentication and access control. We'll
explore why simple password checks aren't enough and build a robust system from
the ground up using Python.

Workshop Outline:

1. Password Strength Analysis
2. Password Hashing Methods
3. Salt and Pepper Implementation
4. TOTP (2FA) Implementation
5. Brute Force Attack Simulation
6. Complete Authentication System

#### Resources

- Password strength
  https://en.wikipedia.org/wiki/Password_strength
- bcrypt is a password-hashing function
  https://en.wikipedia.org/wiki/Bcrypt
- PyOTP Python library
  https://pypi.org/project/pyotp/

## Final Conclusion and Reflection

Completing this lab significantly deepened my understanding of authentication and access control beyond simply “storing passwords securely.” While I had used hashing libraries in the past, I did not fully appreciate the security rationale behind specific design choices. Implementing entropy-based password scoring, dictionary checking, salted hashing, peppers, and TOTP demonstrated how each of these mechanisms addresses a specific threat model rather than being arbitrary security features.

One of the key insights was recognising that security is not a single control, but a layered strategy that slows, limits, and ideally prevents an attacker’s progress at multiple stages. For example, using bcrypt alone is helpful, but combining it with per-user salts, an application-level pepper, and TOTP protects against very different attack vectors such as database leaks, rainbow tables, and brute-force attempts. It was particularly eye-opening to see how quickly MD5 and SHA-256 hashes can be cracked using even a basic dictionary attack.

This lab also highlighted some realistic architectural considerations. The concept of a pepper introduced security beyond cryptography; it forced me to think about where secrets are stored, who controls system configuration, and what happens if different parts of the system are compromised independently. Similarly, implementing TOTP showed me how simple it is to add a second authentication factor, yet how effective it is in practice compared to insecure SMS-based 2FA.

If I were to extend this work further, I would experiment with different bcrypt cost factors to benchmark performance, and generate real provisioning QR codes for authenticator apps.

Overall, this lab shifted my perspective from “how to write secure code” to “how attackers think”. It prompted me to view authentication as an evolving process that must be continuously improved to keep pace with hardware acceleration and ongoing real-world threats.
