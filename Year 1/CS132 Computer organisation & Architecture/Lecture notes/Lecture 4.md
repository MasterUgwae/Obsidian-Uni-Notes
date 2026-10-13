# Introduction to digital logic


- AND
	- f=A.B
	- f=AB
	- f=A$\wedge$B
- OR
	- f=A+B
	- f=A$\vee$B
- XOR
	- f=A$\oplus$B
- NOT
	- f=¬A
	- f=!A
	- f=$\overline A$ 


| A   | B   | AND | NAND |
| --- | --- | --- | ---- |
| 0   | 0   | 0   | 1    |
| 0   | 1   | 0   | 1    |
| 1   | 0   | 0   | 1    |
| 1   | 1   | 1   | 0    |

## gates examples

- 74ls08
	- Chip using and agets
- 74ls32
	- Or gates
- 74ls86
	- xor gates

| A   | B   | C   | P(A.B) | Q(B.C) | R(A.C) | X(P+Q+R) |
| --- | --- | --- | ------ | ------ | ------ | -------- |
| 0   | 0   | 0   | 0      | 0      | 0      | 0        |
| 0   | 0   | 1   | 0      | 0      | 0      | 0        |
| 0   | 1   | 0   | 0      | 0      | 0      | 0        |
| 0   | 1   | 1   | 0      | 1      | 0      | 1        |
| 1   | 0   | 0   | 0      | 0      | 0      | 0        |
| 1   | 0   | 1   | 0      | 0      | 1      | 1        |
| 1   | 1   | 0   | 1      | 0      | 0      | 1        |
| 1   | 1   | 1   | 1      | 1      | 1      | 1        |

So X is true when at least two inputs are true

| A   | B   | C   | P(A.B) | Q(B.C) | R(A.C) | X(P+Q+R) |
| --- | --- | --- | ------ | ------ | ------ | -------- |
| 0   | 0   | 0   | 0      | 0      | 0      | 0        |
| 0   | 0   | 1   | 0      | 0      | 0      | 0        |
| 0   | 1   | 0   | 0      | 0      | 0      | 0        |
| 0   | 1   | 1   | 0      | 1      | 0      | 1        |
| 1   | 0   | 0   | 0      | 0      | 0      | 0        |
| 1   | 0   | 1   | 0      | 0      | 1      | 1        |
| 1   | 1   | 0   | 1      | 0      | 0      | 1        |
| 1   | 1   | 1   | 1      | 1      | 1      | 1        |

$(\overline{A \oplus B}) +(A.¬B.¬C)$
