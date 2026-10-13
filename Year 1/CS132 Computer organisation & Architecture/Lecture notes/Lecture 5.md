# Computer logic 1

## Boolean algebra laws

- De morgan's
	- $\overline A+\overline B=\overline{A.B}$
	- $\overline A.\overline B=\overline{A+B}$
- XOR
	- $A\oplus B=(A+B).\overline{A.B}$


$X=\overline A.\overline B.\overline C+\overline A. \overline B. C+ A. \overline B. \overline C+ A.  B. \overline C+ A.  B. C$
$=\overline A.\overline B.(\overline C+C)+ A. \overline B. \overline C+ A.  B. (\overline C+C)$
$=\overline A.\overline B+ A. \overline B. \overline C+ A.  B$
$=\overline A.\overline B+ A. (\overline B. \overline C+ B)$
$=\overline A.\overline B+ A. (\overline C+ B)$
$=\overline A.\overline B+ A. \overline C+ A.B$
$=\overline{A\oplus B} + A.\overline C$

| A   | B   | C   | A ⊕ B | ¬(A ⊕ B) | ¬C  | A ∧ ¬C | ¬(A ⊕ B) ∨ A ∧ ¬C |
| --- | --- | --- | ----- | -------- | --- | ------ | ----------------- |
| 0   | 0   | 0   | 0     | 1        | 1   | 0      | 1                 |
| 0   | 0   | 1   | 0     | 1        | 0   | 0      | 1                 |
| 0   | 1   | 0   | 1     | 0        | 1   | 0      | 0                 |
| 0   | 1   | 1   | 1     | 0        | 0   | 0      | 0                 |
| 1   | 0   | 0   | 1     | 0        | 1   | 1      | 1                 |
| 1   | 0   | 1   | 1     | 0        | 0   | 0      | 0                 |
| 1   | 1   | 0   | 0     | 1        | 1   | 1      | 1                 |
| 1   | 1   | 1   | 0     | 1        | 0   | 0      | 1                 |

## K-Maps

- Like a truth table but its 2d instead of 1D

| C\AB | 00                                     | 01                            | 11                  | 10                            |
| ---- | -------------------------------------- | ----------------------------- | ------------------- | ----------------------------- |
| 0    | $\overline A.\overline B. \overline C$ | $\overline A. B. \overline C$ | $A. B. \overline C$ | $\overline A. B. \overline C$ |
| 1    | $\overline A.\overline B. C$           | $\overline A. B. C$           | $A. B.  C$          | $A.\overline B. C$            |

$X=A.¬B+A.B$


| A\B | 0   | 1   |
| --- | --- | --- |
| 0   | $0$ | $0$ |
| 1   | $1$ | $1$ |

so $X=1$