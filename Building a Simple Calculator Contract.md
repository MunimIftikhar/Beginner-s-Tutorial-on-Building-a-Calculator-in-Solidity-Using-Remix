# Building a Simple Calculator Contract
Learn how to implement a simple calculator in Solidity.

---

## Select version

Start with selecting the latest version of `pragma solidity`. Let's try adding the following version.

```solidity
pragma solidity >=0.6.0 < 0.9.0;
```

## Creating a contract

Create a solidity contract named `Calculator`.

```solidity
pragma solidity >=0.6.0 < 0.9.0;

contract Calculator {
  // Your code goes here
}
```

## Adding functionalities
Let's add simple arithmetic operations to our calculator.

### Addition
Let's look at the following `addition` function.

```solidity
function addition(uint numberOne, uint numberTwo) public pure returns (uint) {
    return numberOne + numberTwo;
}
```
**Parameters**

`numberOne` and `numberTwo` are two parameters using those we will do addition operation. 

**Access visibility**

The function visibility is `public`, so that we can call
the function and perform the operation. 

**Modifier**

As we are not using any `contract` variable or data from the blockchain, we can simply use `pure` modifier and return 
the result of `numberOne + numberTwo`. 

---

### Subtraction

Let's look at the following `subtraction` function.

```solidity
function subtraction(uint numberOne, uint numberTwo) public pure returns (uint) {
    return numberOne - numberTwo;
}
```
**Parameters**

`numberOne` and `numberTwo` are two parameters using those we will do subtraction operation. 

**Access visibility**

The function visibility is `public`, so that we can call
the function and perform the operation. 

**Modifier**

As we are not using any `contract` variable or data from the blockchain, we can simply use `pure` modifier and return 
the result of `numberOne - numberTwo`. 

---

### Multiplication

Let's look at the following `multiplication` function.

```solidity
function multiplication(uint numberOne, uint numberTwo) public pure returns (uint) {
    return numberOne * numberTwo;
}
```
**Parameters**

`numberOne` and `numberTwo` are two parameters using those we will do multiplication operation. 

**Access visibility**

The function visibility is `public`, so that we can call
the function and perform the operation. 

**Modifier**

As we are not using any `contract` variable or data from the blockchain, we can simply use `pure` modifier and return 
the result of `numberOne * numberTwo`. 

---

### Division

Let's look at the following `division` function.

```solidity
function division(uint numberOne, uint numberTwo) public pure returns (uint) {
    require(numberTwo > 0, "The second parameter should be greater than 0");

    return numberOne / numberTwo;
}
```
**Parameters**

`numberOne` and `numberTwo` are two parameters using those we will do division operation. 

**Access visibility**

The function visibility is `public`, so that we can call
the function and perform the operation. 

**Modifier**

As we are not using any `contract` variable or data from the blockchain, we can simply use `pure` modifier and return 
the result of `numberOne / numberTwo`. 

---
## Final code
After compiling all of the functions inside the `calculator` contract, the code will look like this:

```solidity
pragma solidity >=0.5.0 < 0.9.0; 

contract Calculator {

    function addition(uint numberOne, uint numberTwo) public pure returns (uint) {
        return numberOne + numberTwo;
    }

    function subtraction(uint numberOne, uint numberTwo) public pure returns (uint) {
        return numberOne - numberTwo;
    }

    function multiplication(uint numberOne, uint numberTwo) public pure returns (uint) {
        return numberOne * numberTwo;
    }

    function division(uint numberOne, uint numberTwo) public pure returns (uint) {
        require(numberTwo > 0, "The second parameter should be greater than 0");

        return numberOne / numberTwo;
    }
}
```
