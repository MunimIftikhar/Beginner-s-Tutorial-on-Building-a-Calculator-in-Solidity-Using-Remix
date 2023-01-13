# Setting up a Development Environment
Get introduced to Remix IDE and how can you set it up to run a Solidity program.

---

## What is Remix?

Remix is an IDE (Integrated Development Enviroment). It is an open-source development enviroment, used primarily to run 
Solidity programs and for the entire process of smart contract development.

## Setting up the Remix IDE with Hello, World program
Let's go over the steps how you set up the Remix by writing and deploying your first smart contract.

### Create a new file
Go to the [remix official website](https://remix.ethereum.org), select Solidity and create a new file named `calculator.sol`.

<img width="1439" alt="Screenshot 2023-01-13 at 10 04 56 AM" src="https://user-images.githubusercontent.com/40567828/212246595-3dd3d798-73a5-4983-a4d2-9cf07c9d8dfa.png">

### Run your first program
Copy the following code to the `calculator.sol` file.

````solidity
// SPDX-License-Identifier: UNLICENSED
pragma solidity ^0.8.0;

/**
   * @title Calculator
   * @dev Simple Calculator in Solidity
   * @custom:dev-run-script calculator.sol
   */

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
````
Go to the **File Explorer** and search **Solidity Compiler**. 

<img width="367" alt="Screenshot 2023-01-13 at 4 21 54 PM" src="https://user-images.githubusercontent.com/40567828/212309376-1fde9243-286b-4fcf-a866-ba66992c6425.png">

Click on `Compile and Run Script` button to run the `calculator` contract.

<img width="358" alt="Screenshot 2023-01-13 at 4 25 22 PM" src="https://user-images.githubusercontent.com/40567828/212310016-fc69410d-813b-4041-bef5-18d0f36e2e5b.png">

---
[👉Next Lesson: Deploy and Call the Calculator Contract](https://github.com/MunimIftikhar/Beginner-s-Tutorial-on-Building-a-Calculator-in-Solidity-Using-Remix/blob/main/Deploy%20and%20Call%20the%20Calculator%20Contract.md)
