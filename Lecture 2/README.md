##  PHP Fundamentals

## 1. Variables in PHP and Rules:

Variables in PHP are used to store data values. Here are some key rules for naming variables in PHP:

* Variable names must start with a letter or underscore (_), followed by any number of letters, numbers, or underscores.

* Variable names are case-sensitive.

* PHP variable names cannot contain spaces or special characters, except for the underscore (_).

* PHP variables do not need to be declared before use. They are created when they are first assigned a value.

* Variable names cannot begin with a number.

```php

<?php
// Valid variable names
$varName = "Hello";
$_myVar = 10;
$my_var = "World";

// Invalid variable names
$1var = "Invalid"; // Starts with a number
$my var = "Invalid"; // Contains a space
?>


```


## 2. Data Types in PHP:

PHP supports several data types, including:

* Integer: Whole numbers without decimal points.
* Float (or double): Numbers with decimal points.
* String: Sequence of characters enclosed in quotes (single or double).
* Boolean: Represents true or false.
* Array: Collection of key-value pairs.
* Object: Instances of user-defined classes.
* NULL: Represents a variable with no value.
* Resource: Holds references to external resources.

```php

<?php
// Examples of data types
$intVar = 10; // Integer
$floatVar = 3.14; // Float
$strVar = "Hello, world!"; // String
$boolVar = true; // Boolean
$arrVar = array(1, 2, 3); // Array
$objVar = new MyClass(); // Object
$nullVar = null; // Null
?>

```

## 3. Operators and Operators Types in PHP:

PHP supports various types of operators, including:

* Arithmetic operators: `+, -, *, /, %` (modulus).
* Assignment operators: `=, +=, -=` etc.
* Comparison operators: `==, !=, >, <, >=, <=`.
* Logical operators: `&&, ||, !`.
* Increment/Decrement operators: `++, --`.
* String concatenation operator: `.`


```php

<?php
// Examples of operators
$a = 10;
$b = 5;
$sum = $a + $b; // Arithmetic operator
$isTrue = ($a == $b); // Comparison operator
$andOp = ($a > 0 && $b < 10); // Logical operator
$str = "Hello" . "World"; // String concatenation
?>


```

![Example Image](https://tse4.mm.bing.net/th?id=OIP.miZnJ8QsQL9Bnqh5i6kqFwHaFp&pid=Api&P=0&h=220);
