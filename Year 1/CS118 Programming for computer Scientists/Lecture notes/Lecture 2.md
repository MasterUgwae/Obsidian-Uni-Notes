# Variables, Number Systems & I/O

```Java
/* A java program that uses Euclid’s algorithm to calculate the GCD */
import java.util.Scanner;

public class GCD {
	public static void main (String[] args) {
		Scanner sc = new Scanner(System.in);
		System.out.println("Enter first number: ");
		int a = sc.nextInt(); // input a
		System.out.println("Enter second number: ");
		int b = sc.nextInt(); // input b
		while (a != b) { // while a and b not equal
			// replace larger by the difference…
			if (a > b)
				a = a-b;
			else
				b = b-a;
		}
		System.out.print("The GCD is: "); // then print the result
		System.out.println(a);
	}
}
```


## Classes
```Java
public class S {
	public static void main (String[] args) {
	}
}
```
- S is the name of the file

## Variables
```Java
public class main {
	public static void main (String[] args) {
		[type] name;
	}
}
```
- Variables must be declared with "Type name;"
	- You can write "type name = value;"

## Scanner
```Java
import java.util.Scanner;

public class GCD {
	public static void main (String[] args) {
		Scanner sinput = new Scanner(System.in);
		int a = sinput.NextInt();
	}
}
```

## Output

```Java
public class main {
	public static void main (String[] args) {
		System.out.println("Hello World");
	}
}
```

## Data types

- int is a 32 bit signed integer
	- using two's complement
- byte is an 8 bit twos complement
- short is a 16 bit signed integer
- long is a 64 bit signed integer
- 
- Float IEEE 754 32-bit
	- -3.4e38 to 34e38
	- 6 to 7 significant digits of accuraccy
	- we can specify a float using 3.14f
- Double IEEE 754 64-bit
	- -1.7e308 to 1.7e308
	- Default decimal value
- Bool is 1bit
- Char utf-16 character
	- Stores 65536
	- 


## Equality operators

```Java
/* A java program that uses Euclid’s algorithm to calculate the GCD */
import java.util.Scanner;

public class GCD {
	public static void main (String[] args) {
		while (a == b) { // while a and b not equal
	}
}
```
- == for equality check
- != for not equal check
- > and < are the same as usual


## Streams

- System.in
- System.out
	- Used by system.out.println()
		- output + newline
	- Used by System.out.print()
		- output
- System.err
	- Used by System.err.println()
		- output + newline
	- Used by System.err.print()
		- output

## Concatination
- + concatonates if both operands are strings
	- or if only one is a string

## Type casting
```Java
[type] variable = ([type]) other_variable
```

## Boolean operators

- || OR
- | OR
- && AND
- & AND
- ^ XOR
- ! NOT

## Lazy and strict opertators

- Two symbols means "lazy" and one means "strict"
	- (B || A)
	- If B were true, then it wouldn't be evaluated



> Ask about