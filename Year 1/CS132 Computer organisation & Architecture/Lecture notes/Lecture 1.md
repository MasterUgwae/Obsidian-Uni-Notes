---
tags:
  - CS132
  - intro
---
# Module details
## Lectures

| wk  | Lecture 1                    | Lecture 2                  | Lecture 3                     | Lab                                     |
| --- | ---------------------------- | -------------------------- | ----------------------------- | --------------------------------------- |
| 1   | Numberical representation 1  | Numerical Representation 2 | Numerical Representation 3    | NO LAB                                  |
| 2   | Intrduction to Digital Logic | Computational Logic 1      | Breadboard Exploration (demo) | NO LAB                                  |
| 3   | Computational Logic 2        | Sequential Logic I         | Sequential Logic II           | Intro. to Logic                         |
| 4   | Intro. to Memory Systems     | Errors in Memory Systems   | Long Term Memory              | Logic Identification & Sequential Logic |
| 5   | Intro. to Assembly 01$_2$    | Intro. to Assembly 10$_2$  | Intro. to C                   | Three State Logic & Buses               |
| 6   | Introduction to I/O          | Synchronised I/O           | Interfacing Hardware          | Assembly                                |
| 7   | Processor Architecture 1     | Processor Architecture 2   | Processor Architecture 3      | Software Control                        |
| 8   | RISC & CISC                  | Achieving Performance      | Architecture Comparison       | Hardware Project I                      |
| 9   | Recap Presentations          | Recap: Circuits            | Recap: I/O                    | Hardware Project II                     |
| 10  | Recap: Assembly              | Recap: The Whole Thing     | Future Architecture           | Hardware Project III                    |
## Labs
- 1 2 hour lab per week
- Hardware not available outside of labs
- Labs 1-3 
	- logic gates
- Labs 4-5 
	- Coding with hardware
- Labs 6-8
	- Hardware project
	- Form will open wednesday wk 4

## Assessment
- Coursework 1
	- Worth 15%
	- Due thurday week 8
- Coursework 2 (25%)
	- Due thursday week -
- Final assessment
	- 60%


## Contact details

A.hague@warwick.ac.uk

# History

### Alan Turing
- Developed Mechanical Machines to decipher Enigma
- Developed the stored program concept

## Signals
- First computer only used analogue signals
	- Susceptable to noise
- Digital logic
	- More resilience
	- Cheaper components
	- Smaller components

### Signal Graphs
- Often less smooth than typically drawn
- Drawn as instant voltage change
	- In reality it takes multiple nanoseconds
- 0.8V or less considered a low signal
- 2.8V or more considered a high signal

### Bits, Bytes & Words
- Signals can be shown as bits
	- Low signal = 0 
	- High signal = 1
- 1 Byte = 8 Bits
- [[Glossary/Word|Word]]-> number of bits that can be processed simultaneously
	- Typical word sizes are 16,32 or 64
- [[MSB]]: Bit with the highest value
- [[LSB]]: Bit with the lowest value

### Buses
- Bits can be sent in 2 ways
	- Read over set time intervals
		- Limited to 1 bit at a time
		- Expensive
	- Multiple cables sending a bit each
		- Cheap
		- Easy to extend
- Word size is usually limited to bus size

# Number Representation 1
- Multiple number representation
- For the number 12
	- 12
	- XII
	- A dozen
## Computational Numbers
- Bits are used in base 2
- Other common bases are [[Glossary/Octal|octal]] and [[Glossary/Hexadecimal|hexadecimal]]
- $$3404_{10}=110101001100_2=D4C_{16}=6514_{8}$$
- $value = \sum^{N-1}_{i=0}{symbol_i\times base^i}$

### Word Size
- Bigger the word size -> More computation we can do

### Conversion
1. Divide the number by the base required
2. Record the remainder
3. Repeat

#### Conversion of $163_{10}$-> Binary

| Quotient | Remainder |
| -------- | --------- |
| 163      | ---       |
| 81       | 1         |
| 40       | 1         |
| 20       | 0         |
| 10       | 0         |
| 5        | 0         |
| 2        | 1         |
| 1        | 0         |
| 0        | 1         |
Then read from bottom to top
so $163_{10}=10100011$
## Arithmetic
### Addition/Subtraction
- As learnt in A Level
- [[Glossary/Overflow|Overflow]] is when carry goes past the MSB

### Negative numbers
- Signed Magnitude
	- MSB is used as the indicator

| 1        | 1     | 0     | 1     |
| -------- | ----- | ----- | ----- |
| Negative | $2^2$ | $2^1$ | $2^0$ |
| Yes      | 4     | 2     | 1     |
| -        | 4     | 0     | 1     |
|          |       |       | -5    |
- Two's Complement
	- The MSB represents the negative value of the value

| 1    | 1     | 0     | 1     |
| ---- | ----- | ----- | ----- |
| -2^3 | $2^2$ | $2^1$ | $2^0$ |
| -8   | 4     | 2     | 1     |
| -8   | 4     | 0     | 1     |
|      |       |       | -3    |

- To make a number negative
	- Add a 0 to the left
	- Invert all bits
	- Add 1


Signed magnitude
- Easy to check
- Two values for 0 (+0 and -0)


### Biased form
- Shifts all values by subtracting a constant bias
- It maintains binary ordering

| Bit Pattern | Binary | B=4 |
| ----------- | ------ | --- |
| 000         | 0      | -4  |
| 001         | 1      | -3  |
| 010         | 2      | -2  |
| 011         | 3      | -1  |
| 100         | 4      | 0   |
| 101         | 5      | 1   |
| 110         | 6      | 2   |
| 111         | 7      | 3   |
