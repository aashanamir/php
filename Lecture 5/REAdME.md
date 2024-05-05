#  PHP Functions

Functions in PHP allow you to encapsulate reusable pieces of code, making your code more organized, easier to read, and easier to maintain. In this chapter, we'll explore how to define, call, and use functions effectively in PHP.

## 1. Defining Functions

You can define a function in PHP using the function keyword followed by the function name and a pair of parentheses containing any parameters the function may accept. The function body is enclosed within curly braces {}.

```php
function greet($name) {
    echo "Hello, $name!";
}
```

## 2. Calling Functions

Once a function is defined, you can call it anywhere in your PHP code by using its name followed by parentheses containing any arguments the function requires.

```php
greet("Aashan");
```

## 3. Function Parameters and Return Values

Functions in PHP can accept parameters, which are variables passed into the function when it is called. Functions can also return values using the return statement.

```php
function add($a, $b) {
    return $a + $b;
}

$result = add(3, 4);
echo $result; // Outputs 7
```

## 4. Function Scope

Variables declared inside a function are only accessible within that function and are said to have local scope. Variables declared outside of any function are said to have global scope and can be accessed from anywhere in the script.

```php
$globalVar = "I'm global";

function test() {
    $localVar = "I'm local";
    echo $globalVar; // Accessible
    echo $localVar; // Accessible
}

echo $globalVar; // Accessible
echo $localVar; // Not accessible (will cause an error)
```

## 5. Built-in Functions

PHP comes with many built-in functions that perform common tasks such as string manipulation, array manipulation, date and time handling, and more. These functions can be used directly in your PHP code without the need for additional setup.

```php
$str = "Hello, World!";
echo strtoupper($str); // Outputs "HELLO, WORLD!"
```
## 6. Anonymous Functions

Anonymous functions, also known as closures, allow you to create functions without naming them. They are useful for tasks like callback functions and can be assigned to variables or passed as arguments to other functions.

```php
$greet = function($name) {
    echo "Hello, $name!";
};

$greet("John");
```

Functions are an essential part of PHP programming, allowing you to encapsulate logic, improve code organization, and promote reusability. By defining, calling, and utilizing functions effectively, you can create more modular and maintainable PHP applications. Understanding function scope, parameters, return values, and built-in functions will enable you to leverage the full power of PHP's functional capabilities.