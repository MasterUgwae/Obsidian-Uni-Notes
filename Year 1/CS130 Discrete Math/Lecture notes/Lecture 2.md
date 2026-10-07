---
tags:
  - CS130
---
# Introduction to Sets, Sequences & Functions 2

## Subsets

$$A \subseteq B$$
This means that A is a Subset of B
- If every element that belongs to A also belongs to B
> Glossary
### Examples
- $\mathbb{N}\subseteq\mathbb{Z}$ 
- $\emptyset\subseteq{B},\forall B$
- $\emptyset\subseteq\emptyset$,$A\subseteq A$
- $\mathbb{N}\notin\mathbb{Z}$
- $\mathbb{N}\notin\mathbb{N}$
- $\mathbb{N}\in\{\mathbb{N}\}$

## Cardinality
If there is an n such that $$|A|=n\in\mathbb{N}$$
The set A is finite, otherwise it is infinite

## Specifying sets
- Set builder notation
	- $\{n\in\mathbb{N}:\text{n is prime and}10\leq n\leq100\}$
	- $\{n\in\mathbb{N}|\text{n is prime and}10\leq n\leq100\}$
- $\{n\in\mathbb{Z}:n=m^2\text{ for some }m\in\mathbb{Z}\}$
	- = $\{m^2:m\in\mathbb{Z}\}$
	- = $\{0^2,1^2,(-1)^2,2^2,(-2)^2,...\}$
	- = $\{0,1,1,4,4,9,9...\}$
	- = $\{0,1,4,9,...\}$
	- = $\{n^2:n\in\mathbb{N}\}$
- $\{(-1)^n:n\in\mathbb{Z}\}$
	- = $\{1,-1\}$

## Exercises

1. Find a simpler description of the set $$\{3a+7b:a,b\in\mathbb{Z}\}$$
2. Which of these sets are equal 
$$\begin{gather}
A=\emptyset \\
B = \{\emptyset\} \\
C = \{\{\emptyset\}\}
\end{gather}
$$


## Sequences

### Finite sequences
- $A=\{a,b,c\}$
- $A^2=\{aa,ab,ac,ba,bb,bc,ca,cb,cc\}$
	- $A^2=\{(a,a),(a,b),(a,c),(b,a),(b,b),(b,c),(c,a),(c,b),(c,c)\}$
	- $ac\neq ca$
- $|A^2|=|A|^2$

- Let $G=\{a,aa\}$

- Let $X$ be a set, let  $n\in\mathbb{N}$
- By $X^n$ we denote the set of all sequences of length $n$ of elements of $X$

- notation of the form (a,b) represents an [[Glossary/Ordered Pair|ordered pair]]

$\mathbb{R}^2$ is equivalent to the x,y plane
$[0;1]^2\subseteq\mathbb{R}^2$
