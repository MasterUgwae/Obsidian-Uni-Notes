---
tags:
  - CS130
  - intro
---
# Overview
- Lectures
	- You can find lecture notes on web page
- Seminars
- Coursework
	- Problem sets
		- Worth 10% total
		- Problem set 0 due Monday WK2 
	- January Test/ Class test
		- Worth 10%
- Final Exam
	- In term 3
	- Worth 80%
- Resources
	- [Module information page](https://warwick.ac.uk/fac/sci/dcs/teaching/modules/cs130/)
	- [Online Materials](https://warwick.ac.uk/fac/sci/dcs/teaching/material/cs130/)
	- [Moodle page](https://moodle.warwick.ac.uk/course/view.php?id=78383)
		- Lecture capture on here
	- Books
		- [Reading list](https://rl.talis.com/3/warwick/lists/cd002d1e-f256-4615-b4a0-732a44e562b8.html)

## Questions
- Module forum on [moodle](https://moodle.warwick.ac.uk/my/)
- Office hours
	- Dmitry
		- Tue 14:30 - 1700
		- First come first serve
	- Mattius,
		- Mon 12:00 - 13:00
		- Tue 15:30-16:30
		- Book first
- Email
	- Subject should include module code

Video recordings are released indefinately

# Introduction to Sets, Sequences & Functions

## Notable sets
- Natural numbers: $\mathbb{N}=\{0,1,2,3,\dots\}$
> This includes 0
- Integers: $\mathbb{Z}=\{0,1,-1,2,-2,\dots\}$
- Rationals: $\mathbb{Q}=\{0,1,2,\frac{3}{2},-\frac{3}{2},\dots\}$
- Real Numbers: $\mathbb{R}$
- Complex Number: $\mathbb{C}$
Letters like $\mathbb{N}$ are called blackboard bold
## Notation

### Membership
$$4 \in \mathbb{N}$$
### Exclusion
$$4 \notin \mathbb{N}$$

## Proposition

Sets $A$ and $B$ are **equal** if they contain exactly the same objects.

This means that if for every possible object, it is either contained in both or neither. Then, there is no way to distinguish the sets.

So there is nothing more to a set other than the objects within

Noation: $A=B$

$$
\{a,b\}=\{b,a\}=\{b,a,a\} \neq \{a\} = \{a,a\}
$$
> There is no ordering, and no multiplicity
### Example
Given:
$$
S=\{\mathbb{N},\mathbb{Z},\mathbb{Q},\mathbb{R}\}
$$
Then:
$$
|S|=4
$$
## Cardinality
The empty set is represented by $\emptyset=\{\}$ 

Modulus operator looks like || and is two pipe characters
$$
\begin{gather}
\forall A=\{a,...\} \\
|A|=n
\end{gather}
$$
> Modulus operator returns the size of the set
> The cardinality is the size of the set
> The size of a set is equal to the number of elements within

$$|\emptyset|=0$$
> This is the only set with cardinality 0
