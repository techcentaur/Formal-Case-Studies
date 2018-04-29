## Cryptographic system

Cryptography is an essential part of providing data confidentiality, integrity, and authentication in the security and thus used with similar aim.

## RSA algorithm

In this cryptosystem, the encryption key is public and it is different from the decryption key which is kept private.

RSA algorithm can be categorized in 4 steps:

1. Key generation
	- Choose two distinct prime numbers p and q.
		- p and q should be chosen at random, and should be similar in magnitude but differ in length by a few digits to make factoring harder.
	- Compute n = pq, n is used as the modulus.
	- Compute λ(n) = lcm(λ(p), λ(q)) = lcm(p − 1, q − 1), where λ is Carmichael's totient function. This value is kept private.
	- Choose an integer e such that 1 < e < λ(n) and gcd(e, λ(n)) = 1; i.e., e and λ(n) are coprime.
	- Determine d as d ≡ e−1 (mod λ(n)); i.e., d is the modular multiplicative inverse of e (modulo λ(n)).
	- e is released as the public key exponent.
	- d is kept as the private key exponent which must be kept secret alongwith p, q and λ(n).

2. Key Distribution

	- For using public key, polling booth administration gives the (n, e) which can be use to encrypt data.
	- For decryption, (d) is preserved at Election Commission administration.

3. Encryption
	-  c = mod(m^e /n) where m is the integer corresponding to the plaintext that we want to encrypt.

4. Decryption
	- c^d = mod((m^e)^d / n), given d, it is easy to decrypt the required integer m, which can be converted into plaintext.

## 