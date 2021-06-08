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
```

Will output:

```
5
7
```

Whereas

```
x = 5
print(x)
print(x)
x = 7
```

Will output:

```
5
5
```

#### Arithmetic in Python

Now that we know how to assign integers (whole numbers) to variables, we can perform simple arithmetic using these variables.

Let's take two variables, `x` and `y` and assign them different integer values:

```
x = 5
y = 7
```






