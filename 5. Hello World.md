# Hello World
Learn to write Hello, World in Solidity.

---

## Code
Let's look at the following `Hello, World!` program in Solidity.

```solidity
pragma solidity ^0.8.0;

contract HelloWorld {

    function print () public pure returns (string memory) {       
        return 'Hello, World!';             
    } 
}
```

## Explanation
Let's break down the code line by line and understand it.

### Pragma

As we have discussed, `pragma solidity ^0.8.0;` is used to tell the console to use the specific version of Solidity.

`^` indicates using a version greater than `0.8.0`.

### Contract

The `contract HelloWorld` declares a contract named `HelloWorld`.

### Function

The `function` keyword declares a function named `print`, that is public and has a `pure` access modifier.
`returns (string memory)` defines the return type as a string coming from the blockchain memory.
The `pure` modifiers specify that function does not need to access any data or variable declared in a contract.

---
[👉Next Lesson: Build a Simple calculator Contract](https://github.com/MunimIftikhar/Beginner-s-Tutorial-on-Building-a-Calculator-in-Solidity-Using-Remix/blob/main/Build%20a%20Simple%20Calculator%20Contract.md)
