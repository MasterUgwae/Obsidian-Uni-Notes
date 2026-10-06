---
tags:
  - CS132
---
# Multiplication

- In unsigned binary it is the same as decimal

## Multiplication algorithm
1. Set a counter to n (number of bits)
2. Set 2n-bits partial product to 0
3. Check if LSB of multiplier is 1
4. If it is, add multiplicand to n most significant bits, othewise do nothing
5. Right shift Partial product
6. Right sift multiplier
7. Decrement counter
8. repeat

## Multiplication in signed binary
- For signed Magnitude
	- exclude the MSB
	- Multiply the rest as before
	- XOR the MSB to  become the new sign
- For Two's complement use [[Glossary/Booth's Algorithm|Booth's Algorithm]]

