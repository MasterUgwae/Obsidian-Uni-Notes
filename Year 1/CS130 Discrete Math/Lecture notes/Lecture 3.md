# Introduction to Sets, Sequences and Functions 3
## What is a function?

- A function maps one set to another set
	- $f.X\rightarrow Y$
		- the function f maps from X(domain) to Y (co-domain)
- Definition:
	- Let $X$ and $Y$ be sets
	- Suppose there is a rule that specifies,
	- for every element $x\in X$, an unambiguously determined element $y\in Y$; then we say there is a function from $X$ to $Y$.
	> Add to glossary

- $y=f(x)$ for $x\in X$
	- then $y$ is **the** image of $x$ under $f$
	- And $x$ is a preimage of $y$ under $f$
- The range of $f$ is the set:
	- Range$(f)=\{y\in Y:y=f(x)$ for some $x\in X\}=\{f(x):x\in X\}$
	- it is always a subset of the co-domain

## Examples of functions
$f.X\rightarrow Y$
1. If $S$ is the set of all students at Warwick and $U$ is the set of all staff members at Warwick
	- for each, $s\in S$,
	- Let $t(s)\in U$ be the personal tutor of $s$
	- Now $t:S\rightarrow U$
2. $X=\{a,b,c\}, Y=\{d,e,f\}$
	-  s 

| $x$ | $h_1$ | $h_2$ |     |
| --- | ----- | ----- | --- |
| a   | d     | f     |     |
| b   | e     | f     |     |
| c   | f     | f     |     |
3. $E=\{0,1\}^2, G=\{0,1\}$
	- $E\rightarrow G$

| $e$ | $g$ |
| --- | --- |
| 0,0 | 0   |
| 0,1 | 0   |
| 1,0 | 0   |
| 1,1 | 1   |
4. $f:\mathbb{R}^2\rightarrow\mathbb{R}$
	1. $f((x,y))=\sqrt{x^2+y^2}$
5. $g$
	1. $g((x,y))=x+y$
6. $g((x,y))=y$
7. $f:{a,b,c}\rightarrow \mathbb{R}$
	1. f(a)=5
	2. f(b)=4
	3. f(c)=3
	4. range(f)=\{3,4,5\}
8. $sign:\mathbb{R}\rightarrow\{-1,0,1\}$
	1. sign(x)=1, for every x>0
	2. sign(x)=-1, for every x<0
	3. sign(x)=0, for x=0
	$$sign(x)=\begin{cases}
sign(x)=1, for every x>0 \\
sign(x)=-1, for every x<0 \\
sign(x)=0, for x=0 \\
\end{cases}
$$

## Are these real to real

- $f_1(x)=\frac{1}{x}$
	- not a functgion from r to r
- $f_2(x)=\sqrt{x}$
	- not real to real
- $f_3(x)=\pm\sqrt{x^2+1}$
	- not unambiguous