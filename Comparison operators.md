Comparison operators in PHP are used to compare values and determine the relationship between them. These operators evaluate expressions and return a Boolean result (either true or false) based on the comparison's outcome. Here are the commonly used comparison operators in PHP:

1. Equal (==): This operator checks if two values are equal, regardless of their data types. For example:

```php
$a = 10;
$b = "10";
$result = ($a == $b); // true
```

2. Identical (===): The identical operator compares both value and data type. It returns true only if both the value and data type of the operands are the same.

```php
$a = 10;
$b = "10";
$result = ($a === $b); // false
```

3. Not Equal (!=): This operator checks if two values are not equal. It returns true if the values are different.

```php
$a = 5;
$b = 10;
$result = ($a != $b); // true
```

4. Not Identical (!==): The not identical operator checks if both the value and data type of the operands are not the same.

```php
$a = 5;
$b = "5";
$result = ($a !== $b); // true
```

5. Greater Than (>): This operator checks if the left operand is greater than the right operand.

```php
$a = 10;
$b = 5;
$result = ($a > $b); // true
```

6. Less Than (<): This operator checks if the left operand is less than the right operand.

```php
$a = 5;
$b = 10;
$result = ($a < $b); // true
```

7. Greater Than or Equal To (>=): This operator checks if the left operand is greater than or equal to the right operand.

```php
$a = 10;
$b = 10;
$result = ($a >= $b); // true
```

8. Less Than or Equal To (<=): This operator checks if the left operand is less than or equal to the right operand.

```php
$a = 5;
$b = 10;
$result = ($a <= $b); // true
```

Special Comparison Operator - Spaceship Operator (<=>):
The spaceship operator was introduced in PHP 7 and is used for combined comparison. It compares two expressions and returns:

- 0 if both expressions are equal.
- 1 if the left expression is greater.
- -1 if the right expression is greater.

```php
$a = 5;
$b = 10;
$result = ($a <=> $b); // returns -1
```

The spaceship operator is useful for sorting and comparing arrays.

Keep in mind that when using comparison operators, be cautious of the data types being compared, especially with "==" and "===", as their behavior can sometimes lead to unexpected results. It's generally safer to use the identical operator "===" when you want to ensure both value and data type are the same during comparison.
