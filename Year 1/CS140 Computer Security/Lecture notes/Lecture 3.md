
## Basic terminology

- Asset 
	- Anything you want to protect
- Vulnerablility
	- A flaw or weakneess in a system that could be exploited.
- Threat
	- A potential for violation of security.
	- It is when an attacker has both capability and intention
- attack
	- An assult on security in which a threat actor exploits vulnerability to realise the threat
- Risk
	- An expectation of loss expressed as the probability of an attack occuring x loss
- Countermeasure
	- An action that reduces a threat vulnerabililty, loss by eliminating or preventing ot detecting the attack.
- Trust
	- 

## Risk analysis methods
- Qualitative analysis
	- Using a checklist
	- DREAD model by microsoft is an example
		- Damage
		- Reproducability
		- Exploitability
		- Affected User
		- Discoverability
	- Damage vs affected users
		- Damage is the severity per victim
		- Affected users is the scope of the attack
- Quantitative risk analysis
	- Fault tree analysis

## Strategies to handle risks

- Fix the vulnerability
- Risk acceptance
- Risk avoidance
- Risk transference
- Detection
- Reaction

# Public Key Encryption

Based on one way functions
-  Given the input of the function, it is easy to calculate the output
- Givent the output, it is hard to calculate the input

## Modular Arithmetic
### Congruence
- If a and b are equal to the same remainder after division by n, they are said to be congruent
- $a\equiv b \space mod \space n$
- any number is congruent to infinitly many numbers

### Properties

- $(A+B)\space mod \space n\equiv((A\space mod \space n)+B)\space mod\space n$
- $(A+B)\space mod \space n\equiv A\space mod \space n+B\space mod\space n$
- $(A\times B)\space mod \space n\equiv((A\space mod \space n)\times B)\space mod\space n$
- $(A\times B)\space mod \space n\equiv A\space mod \space n\times B\space mod\space n$
- $x^{A*B} \space mod \space n\equiv(x^A\space mod \space n)^B\space mod \space n$
- $(x^A\space mod \space n)^B\space mod \space n\equiv(x^B\space mod \space n)^A\space mod \space n$
#### Examples
- $(48+74)mod 5$
	- $(48+74)\equiv122\equiv2mod5$
	- $(48+74)=3+4=2mod5$
- $5^{12}\space mod \space17$
	- $\equiv 5^{3*4}\space mod \space17$
#### Exercise
1. 2
2. x=5

### Modular exponentiation

- $y^x\space mod \space n$ for different values of x repeats with order n
- If all numbers from 1 to (n-1) we call it a primative root

$3^7mod 7=3^6mod7*3mod7$
This will only apply when the modulo is a prime

- if y is the primative root mod p, then
	- successive powers of y mod p, for x=1 to p-1 generate all numbers from 1 to p-1 mod p

	k=y^x mod p is a one-way function, if
		y is the primative root mod p
		p is an enourmous number, eg 512 bit number

## RSA 

### Notation
- KP_x is the user private key
- KU_x is the public key
- Plaintext - unencrypted message
- Ciphertext - encrytped message
### Encryption
- Bbo chooses 2 large secret primes p and q and calculates n=p*q
- Public key consists of two components: n is the modulus of the public key
- It also needs an exponent
	- Conditions for selecting e
	- $\phi$(n)=(p-1)*(q-1)
		- e is coprime to $\phi(n)$
		- (p-1)\*(q-1)= p*q-p-q = how many integers are coprime to n
	- $1<e<\phi(n)$
Example:
- p=17, q=11, n=187


$$\{x^3|x\in\mathbb{Z}\wedge -4\le x\le4\}$$