# Lesson 02

## Key Terms

* **Comment**: Any line prefixed with a symbol that indicates that the line should not be interpreted as code by the computer (these can be especially helpful to explain in our own words what a piece of code does, so we do not forget later). In Python, we use the `#` symbol
* **Variable**: A storage location with a name, that contains some data (the data of which can be subject to change)
* **Function**: Way of compartamentalizing/organizing code, that "takes in" some data as input, and "returns" some output
* **Data Structure**: A format for organizing computer data
* **Integer**: A data structure that represents any whole number 

## Lesson

### Variables and Variable Assignment

#### Assigning Integer Values

The below code will "assign" the value `5` to the variable `x`

```
x = 5
```

The syntax is `<variable_name> = <data_value>`. Spaces before and after the `=` sign are not necessary, so another valid syntax is:

```
x=5
```

We can change the value assigned to `x` by typing the same code but changing the data value:

```
x = 7
```

To check the value of `x` at any point in our code, we can print it on the commandline using:

```
print(x)
```

**Note**: Code is interpreted by the computer procedurally, one line at a time. To check the value of `x`, we should put the print statement *after* the line in which it is assigned. E.g.

```
x = 5
print(x)
x = 7
print(x)

>> 5
>> 7
```

Whereas the following code will simply print `5` twice:

```
x = 5
print(x)
print(x)
x = 7

>> 5
>> 5
```

#### Arithmetic in Python

Now that we know how to assign integers (whole numbers) to variables, we can perform simple arithmetic using these variables.

Let's take two variables, `x` and `y` and assign them different integer values:

```
x = 5
y = 7
```

Basic arithmetic operators in Python are: **addtion (+), subraction (-), multiplcation (\*), division (/), and modulus (%)**

To add together `x` and `y` and assign the result to a new value, we could do the following:

```
z = x + y
print(z)

>> 12
```

We do not need to use variables to do arithmetic, and the below code will have the same result:

```
z = 5 + 7
print(z)

>> 12
```

In fact, we do not even need to assign a variable, if all we want to do is print the result of this addition in the terminal:

```
print(5 + 7)

>> 12
```

Note that Python follows standard order of operators (PEMDAS) as in mathematics, when evaluating longer arithmetic expressions:

```
z = 7 + (6 × 5 + 3)

>> 40
```

#### The modulo operator

The modulo operator returns the remainder after dividing one number by another.

```
print(6 % 5)

>> 1
```

`6 / 5` will have a remainder of 1.

```
print(6 % 3)

>> 0
```

`6 / 3` will have no remainder.


#### Other data structures

So far, we have been assigning variables and performing arithmetic using integer data structures (or data types). There are infinitely many possible data structures, and we can even create our own. However, there are 4 basic data structures that are the building blocks of Python:

* String
* Float
* Boolean
* Integer

A string is any text, and can be specified by the syntax of surrounding characters with `''` or '""`

```
my_string = 'hello world 123'
print(my_string)

>> hello world 123
```

A float or floating-point number is a decimal number. We can perform arithmetic with floats the same way we did with integers.

```
my_float = 0.123
print(my_float)

>> 0.123
```

A boolean is one of two values: True or False, and is the most basic data type.

```
my_bool = True
print(my_bool)

>> True
```

### Introducing functions

Functions take in some data, and use it to generate some output. The `print` function, for example, takes in any data type, and returns it on the commandline. The syntax for a function is: `<function_name>(<data_1>, <data_2>, <data_3>, ...)`. That is, the data will be entered within parantheses, following the function name.

A function can take one or many values as input.

Example: `print(100)` or `my_function(1, 2, 3, 4, 5)`

The `print` function, specifically, takes a single input, in the examples we have gone over so far

#### Introducting to string manipulation

Python offers many ways to manipulate strings. For example, we can combine strings using the `+` operator:

```
print('hello' + 'world')

>> helloworld
```

Note that the `+` operator is interpreted as addition when comparing integers or floats, but does something entirely with strings: it concatenates, or combines them.

What would happen if we tried combining a string with an integer or a float, however?

```
print('hello' + 123)


>> Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: cannot concatenate 'str' and 'int' objects
```

We would actually get an error that complains that strings and integers cannot be combined. Instead, we would either have to put `123` in quotes to express it as a string:

```
print('hello' + '123')

>> hello123
``

Or we could use the built in `str()` method to convert `123` to a string when we need to:

```
print('hello' + str(123))

>> hello123
```

Some other ways of expressing this using variables would be:

```
hello = 'hello'
onetwothree = 123
string_onetwothree = str(123)

print(hello + string_onetwothree)

>> hello123
```

Or:

```
hello = 'hello'
string_onetwothree = str(123)

print(hello + string_onetwothree)

>> hello123
```

This can be useful when we want to perform arithmetic on a numeric value *before* converting it to a string and printing it out:

```
x = 5
y = 7

z = x + y

print('Result of z: ' + str(z))

>> Result of z: 12
```

## Practice questions

* Do you need to assign numbers to variables to perform arithmetic on them?
* What happens when you try to use `+` to combine strings and integers/floats? How can we resolve this?
* What will `5 % 2` print?
* Can you find a way to print the result of `5 * 2 / 5` using one line of code?
* Does Python follow PEMDAS for arithmetic?
* What function converts integers and floats to strings, and how do we use it?
* What kind of quotes need to be used to create a string data type?

