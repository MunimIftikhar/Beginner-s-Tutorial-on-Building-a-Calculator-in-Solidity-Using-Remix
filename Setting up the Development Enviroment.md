# Setting up the Development Enviroment
Get introduced to Remix IDE and how can you set it up to run a Solidity program. Write Hello, World program and deploy it on Ethereum blockchain.

---

## What is Remix?

Remix is an IDE (Integrated Development Enviroment). It is an open-source development enviroment, used primarily to run 
Solidity programs and for the entire process of smart contract development.

## Setting up the Remix IDE with Hello, World program
Let's go over the steps how you set up the Remix by writing and deploying your first smart contract.

### Create a new file
Go to the [remix official website](https://remix.ethereum.org), select Solidity and create a new file named `helloworld.sol`.

<img width="1439" alt="Screenshot 2023-01-13 at 10 04 56 AM" src="https://user-images.githubusercontent.com/40567828/212246595-3dd3d798-73a5-4983-a4d2-9cf07c9d8dfa.png">

### Run your first program
Copy the following code to the `helloworld.sol` file.

````solidity
pragma solidity ^0.8.0;

contract HelloWorld {

    function print () public pure returns (string) {       
        return 'Hello, World!';             
    } 
}
````
Your `helloworld.sol` file will look like this.

<img width="484" alt="Screenshot 2023-01-13 at 11 37 49 AM" src="https://user-images.githubusercontent.com/40567828/212254008-455b1e6d-aec1-4bf8-9715-0c6ce03a1ade.png">

