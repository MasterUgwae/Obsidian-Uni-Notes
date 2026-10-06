

# Method
1. Unpack Numbers
2. Set cycle counter
3. Clear partial product
4. Test Current multiplier bit ad next loewr order bit
	1. If multiplier bit =0 and next lower bit = 1
		1. Add multiplicand to partial product
	2. Both Multiplier and the lower bit are the same
		1. Do nothing
	3. If multiplier bit = 0 and next lower bit = 1
		1. Subtract multiplicand from partial product
5. Arithmetic right shift partial product and select next pair of multiplier bits
6. Decrement counter
7. Repeat