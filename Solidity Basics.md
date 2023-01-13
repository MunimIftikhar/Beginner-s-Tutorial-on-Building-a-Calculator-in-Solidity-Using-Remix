# Solidity Basics
An overview of Solidity's basic data types, variables, comments, if-else, while loop, for loop, and functions.

## Solidity variables
Variables are declared inside the contract. The basic syntax of declaring a variable is as follows:
```
dataType visibilitySpecifier variableName
```
### Example
```solidity
uint public num;
```

## Solidity visibility specifiers
Visibility specifiers specify where variables or functions can be accessible. Following are some of the visibility specifiers in Solidity.

* `public`: Public functions or variables are accessible by `internal` and `external` contracts.
* `private`: Private functions or variables are only accessible by `internal` contracts.
* `external`: External functions or variables are only accessible by `external` contracts.
* `internal`: Internal functions or variables are only accessible by `internal` contracts or inherited contracts.

## Solidity data types
Some of the solidity data types are as follows:
* `bool`: Used to define `true`/`false` values.
* `string`: Donated using single or double quotes.
* `uint`: Used to define unsigned integers
* `int`: Used to define signed and unsigned integers

## Solidity comments
Solidity comments work the same as C++ comments. We can use `//` for single-line comments and `/* */` for multiple-line comments.

## Solidity if-else
The basic syntax of if-else in Solidity is as follows:
```solidity
if (condition) {
    // Code block
}
else {
   // Code block
}
```

## Solidity while loop
While loop in Solidity works the same as C++.
```solidity
while (condition) {
  // code block
}
```

## Solidity for loop
The basic syntax of a for loop in Solidity is as follows:
```solidity
for (initialization; condition; iteration) {
  // code block
}
```

## Solidity functions
We can declare functions using the `function` keyword in Solidity. The basic syntax of a function in Solidity is as follows:
```solidity
function FunctionName (parameters if-any) <visiblity specifier> <modifier> returns (return type) {
  // code block
}
```

## Solidity access modifiers
Access modifiers define the behavior of the function. They help the contract to identify or change the state of the data.
Following are some of the access modifiers in Solidity.
* `constant`
* `pure`
* `view`
* `payable`

---
[👉Next Lesson: Hello World](https://github.com/MunimIftikhar/Beginner-s-Tutorial-on-Building-a-Calculator-in-Solidity-Using-Remix/blob/main/Hello%20World.md)
