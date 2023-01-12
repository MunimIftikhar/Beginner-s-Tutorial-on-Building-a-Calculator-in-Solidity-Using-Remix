# What is a Contract in Solidity?
Get an understanding of contracts in Solidity. What are they, how are they structured, and how can they be implemented? 

## What is a contract in Solidity?
Solidity contracts work like a class in any object-oriented programming language, e.g., Java and C++. 
A contract has the following properties, just like classes:
* Constructor
* Variables
* Functions

## Contract syntax

Let’s look at the basic syntax of a contract in Solidity:

```solidity
pragma solidity >=0.6.0 <0.9.0;

contract example {
  // Variables declaration
  // Constructor declaration
  // Functions declaration
}
```

### Pragma

Pragma works like an identifier, that identifies the code is written in Solidity.
Pragma helps prevent the breakage for future newer versions. It helps specify the version and load functionalities accordingly.
Pragma also tells the compiler about how to run the code. That is why each Solidity sourse code should start with `pragma version` line.

### Contract keyword
The `contract` keyword helps declaring the contract in Solidity that enclose the code: constructor, variables, functions.
