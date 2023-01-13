# Hello, World
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
Let's try breaking down the code line by line and understand it.

### Pragma

As we have discussed before, `pragma solidity ^0.8.0;` is used to tell the console to use the specific version of Solidity.

`^` indicates to use the version greater than `0.8.0`.

### contract

The `contract HelloWorld` declares a contract named `HelloWorld`.

### Function

The `function` keyword decrales a function named `print`, that is public and has `pure` access modifier.
`returns (string memory)` defines that the return type is string that is coming from the blockchain memory.
The `pure` modifiers specifies that function does not need to access any data, any variable declared in a contract.
