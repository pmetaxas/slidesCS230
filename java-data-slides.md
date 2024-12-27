# Data and Expressions in Java

---

# String Fundamentals
- Character strings are objects in Java (String class)
- String literals are enclosed in double quotes
- Two key printing methods:
  - `System.out.print()` - prints without line break
  - `System.out.println()` - prints with line break
- String concatenation using + operator
  - Combines strings with other strings or data types
  - Example: `"The answer is " + 42`
- Escape sequences for special characters:
  - `\n` - newline
  - `\t` - tab
  - `\"` - double quote
  - `\\` - backslash

---

# Variables and Data Types
- Variables: Named memory locations that store values
- Declaration syntax: `type variableName;`
- Eight primitive data types:
  - Integers: byte, short, int, long
  - Floating point: float, double 
  - char: Single Unicode character
  - boolean: true/false values
- Constants declared with final keyword:
  ```java
  final int MAX_SCORE = 100;
  ```
- Strong typing: Variables must be declared with specific type

---

# Expressions and Operators
- Arithmetic operators:
  - Basic: +, -, *, /, % (remainder)
  - Increment/decrement: ++, --
- Operator precedence:
  1. Parentheses ()
  2. Multiplication, Division, Remainder
  3. Addition, Subtraction
- Assignment operators:
  - Basic assignment: =
  - Combined operators: +=, -=, *=, /=
- Integer vs floating point division:
  - 5/2 = 2 (integer division)
  - 5.0/2 = 2.5 (floating point division)

---

# Type Conversion
- Widening conversions (safe):
  - byte → short → int → long → float → double
  - No data loss
  - Happens automatically
- Narrowing conversions (unsafe):
  - May lose data
  - Requires explicit casting
  ```java
  double price = 19.99;
  int dollars = (int)price;  // becomes 19
  ```
- String conversion:
  - Numbers automatically convert when concatenated
  - Example: `"Price: $" + 19.99`

---

# Interactive Input
- Scanner class used for reading input:
  ```java
  import java.util.Scanner;
  Scanner scan = new Scanner(System.in);
  ```
- Key input methods:
  - `nextInt()` - reads integer
  - `nextDouble()` - reads decimal number
  - `next()` - reads single word
  - `nextLine()` - reads entire line
- Example usage:
  ```java
  System.out.print("Enter value: ");
  int value = scan.nextInt();
  ```
