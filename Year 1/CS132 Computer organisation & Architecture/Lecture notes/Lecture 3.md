# Numerical representation 3

## Fixed point
- Qn/f
	- n is the number of bits for the whole part
	- f is the number of bits for the fractional part

## Floating point
- 1 bit for sign
- 8 bits for exponent
- 23 bits for mantissa/significand
- no two's  complement

| IEEE Standard | Half Precision | single precision | double precision | quad precision |
| ------------- | -------------- | ---------------- | ---------------- | -------------- |
| Sign          | 1bit           | 1 bit            | 1 bit            | 1 bit          |
| Exponent      | 5              | 8                | 11               | 15             |
| Significand   | 10             | 23               | 52               | 112            |
| Bias          |                |                  |                  |                |

## Arithmatic
- Match the exponents
- Add the significands together
- renormalise

Algorithm in lecture slides