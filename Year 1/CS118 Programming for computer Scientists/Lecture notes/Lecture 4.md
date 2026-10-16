
# COntrol Flow

## If Statements
```java
if (booleanExpression) {
	Statement;
	Statement;
}
```
> curly braces not required if only one statement is in the if statement

```java
 if (booleanExpression) 
	Statement;

```

### If..Else
```java
if (booleanExpression) {
	Statement;
	Statement;
} else {
	Statement;
}
```
### Nested
```java
if (booleanExpression) {
	Statement;
	Statement;
} else {
	if (booleanExpression) {
		Statement;
	} else {
		Statement;
	}
}
```
### If..Else If..Else

```java
if (booleanExpression) {
	Statement;
	Statement;
} else if (booleanExpression) {
	Statement;
} else {
	Statement
}
```


### Example
```java

if (mark < 40) {
	classification = "fail";
} else if (mark < 40) {
	classification = "Third";
} else {
	Statement
}
```

```java

if (x < 40)
	if (y < 40) 
		System.out.println("x and y are less than 40");
else 
	Statement
```
the ```else ``` statement belongs to the nested if statement


## Ternary operator
```java
value = (booleanCondition) ? valueIfTrue : valueIfFalse;

int j = (x<5) 1 : 2
```

## Switch Statements
```java
switch (variable) {
	case VALUE:
		Statement;
		break;
	case VALUE:
		Statement;
	default:
		Statement;
}
```
**THERE IS FALL THROUGH**
- Use ```break``` to prevent fallthrough
### Switch Expressions

```java
public static int checkValue(String rarity){
	int val = switch (rarity) {
		case "Common" -> 1;
		case "Uncommon" -> 2;
		case "Rare" -> 3;
		case "Super Rare" -> 4;
		default -> {
			if (rarity.length() < 4) yield -1;
			else yield -2
		}
	}
	
	return val
}
```

- Yield in this case is to set the value of val and not the function return


