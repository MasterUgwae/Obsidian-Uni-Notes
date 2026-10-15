# Predicate Logic & Quantifiers

## Quantifiers
- Existential: $\exists x\in S: p(x)$
- Universal: $\forall x \in S:p(x)$

> Variable names don't matter
> But: **Don't use the same variable name twice in the same formula!**


### Laws for quantifiers
> Don;t hold for empty variable ranges

- $(\forall x:True)\iff True,(\exists x:True)\iff True$
- $(\forall:False)\iff False$,$(\exists:False)\iff False$
- $(\forall:p(x))\implies(\exists x:p(x))$
- Quasi-De Morgan:
	- $¬(\forall x:p(x))\iff(\exists x:¬p(x))$
	- $¬(\exists x:p(x))\iff(\forall x:¬p(x))$

> In General,
> $(\exists x:p(x))\wedge(\exists x:q(x))\neq \exists x:(p(x)\wedge q(x))$
> $(\forall x:p(x))\vee(\forall x:q(x))\neq \forall x:(p(x)\vee q(x))$
> The other way does work
> $\exists$ works with $\vee$
> $\forall$ works with $\wedge$


If one predicate with a variable $x$ but the other one doesn't, then the rules that you guess typically work out:
- $(\forall x:p(x))\vee q\iff \forall x:(p(x)\vee q)$
- $(\exists x:p(x))\wedge q\iff \exists x:(p(x)\wedge q)$
- $(\forall x:p(x))\vee q(y)\iff \forall x:(p(x)\vee q(y))$
- $(\exists x:p(x))\wedge q(y)\iff \exists x:(p(x)\wedge q(y))$

### Practice round
1. $¬(\exists x :p(x))$
	1. $\nexists x :p(x)$
2. Write "there is exactly one x"
	1. $\exists x:(p(x)\wedge (\nexists y:(y\neq x)\wedge p(y))))$
	2. $\exists!x:p(x)$ 

# Introduction to proofs

## Proof Strategies
- Direct Proof:
	- For theorums of the form $p\implies q$
	- we can try a direct proof.
	- Only the highlighted part of the 

| P   | Q   | $P\implies Q$ |
| --- | --- | ------------- |
| F   | F   | T             |
| F   | T   | T             |
| ==🔴T==   | ==🔴F==   | ==🔴F==             |
| ==🔴T==   | ==🔴T==   | ==🔴T==             |
- . 
	- Because of this a theoruen with a directr proof looks like this
		- Theorem: $p\implies q$
		- Proof: Suppose $p$
		- Then ...
		- Therefore, q
		- Q.E.D
	- Example:
		- Theorem: $\forall x\in\mathbb{Z},if 5x+3$ is odd then x is even
		- Proof: Suppose 5x+3 is odd
		- Then 
			- $(5x+3)-3=5x$
			- As 5x+3 is odd and 3 is odd then 5x is even.
		- then $\mathbb{Z}\ni x=\frac{5x}{5}$
			- is even as the quotient of an even and an odd integer 