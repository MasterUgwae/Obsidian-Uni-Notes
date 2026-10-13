# Propositional logic

## Building blocks

- Propostions
	- Atomic
		- Statement that have a truth value
			- eg. pigs can fly
		- p,q,r or A, B, C
	- Compound
		- Statements that are built upon atomic propositions
		- built with logical connectors
		- 
	- Examples of connectors
		- negation ¬ P
		- Conjunction P$\wedge$ Q
		- Disjunction  p$\vee$Q
		- Implication P $\implies$ Q
		- equivalence P $\iff$ Q

Statements have a truth value in $\mathbb{B}=\{F,T\}$
Logical connectors are function from $\mathbb{B}^k \rightarrow \mathbb{B}$ for finite $k$ 

### Truth tables
For negation

| P   | ¬P  |
| --- | --- |
| F   | T   |
| T   | F   |

For the rest

| P   | Q   | $P\wedge Q$ | $P\vee Q$ | $P\implies Q$ | $P\iff Q$ |
| --- | --- | ----------- | --------- | ------------- | --------- |
| F   | F   | F           | F         | T             | T         |
| F   | T   | F           | T         | T             | F         |
| T   | F   | F           | T         | F             | F         |
| T   | T   | T           | T         | T             | T         |

#### Example
$(p\implies q)\iff(¬q\implies¬p)$

This can be reprensented as a tree

- $\iff$
	- $\implies$
		- p
		- q
	- $\implies$
		- ¬
			- q
		- ¬
			- p

| P   | Q   | $(p\implies q)\iff(¬q\implies¬p)$             |
| --- | --- | --------------------------------------------- |
| F   | F   | T                    T      T       T      T  |
| F   | T   | T                   T        F      T      T  |
| T   | F   | F                    T       T       F      F |
| T   | T   | T                   T        F       T      F |

### Tautology
A tautology is a proposition that is true for all truth values of atomic propositions

### Logical equivalences

p and q are logically equivalent written($p \equiv q$)