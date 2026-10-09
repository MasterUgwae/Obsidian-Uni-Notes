---
tags:
  - CS118
---
# Introduction

## Assessment
- 2 hour examination
	- worth 60%
	- week 1 or 2 of term 3
- coursework
	- 2 Programming assignments
		- 1 due week 5
		- 1 due week 10
	- worth 40%

## Reading
- [Introduction to java programming by Y daniel liang](https://warwick.summon.serialssolutions.com/#!/search?pn=1&ho=t&include.ft.matches=f&l=en-UK&bookMark=eNqNyksOwiAUAEAS68JP7_AuYMKnEbo2GnXtvnkCEmILBqi9vhzB7WS2pAkx2BVpe6kY73lHORN0Q7pbKCmaWRcfA5QId_wifFJ0CafJBwcYDBgsCLmk2uZk856sXzhm25Kmmt0RuJwfp-thwbR4_R507WN0w1NIJo-KKvFH-QGKPzG0)
- Moodle forum

## Contact info
- James Archmbold
	- MB3.21 1:30-2:30  monday/thursday
	- james.archbold@warwick.ac.uk
- Ayse Sunar
	- CS3.31
	- ayse.sunar@warwick.ac.uk

## Example of Java code for GCD algorithm

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

