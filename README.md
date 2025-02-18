# solidity-examples
Solidity Examples and Explanations. Examples are from [this site](https://solidity-by-example.org/hello-world/)


## HelloWorld Smart Contract

This repository contains a simple Solidity smart contract that stores and returns a greeting message.

## Solidity Code

```solidity
// SPDX-License-Identifier: MIT
// Compiler version must be greater than or equal to 0.8.26 and less than 0.9.0
pragma solidity ^0.8.26;

contract HelloWorld {
    string public greet = "Hello World!";
}
```

## Explanation

### License Identifier
```solidity
// SPDX-License-Identifier: MIT
```
- This specifies that the contract is licensed under the **MIT License**.

### Solidity Compiler Version
```solidity
pragma solidity ^0.8.26;
```
- The contract is compatible with Solidity version **0.8.26 or higher**, but **below 0.9.0**.

### Contract Declaration
```solidity
contract HelloWorld {
```
- Defines a Solidity smart contract named `HelloWorld`.

### State Variable
```solidity
string public greet = "Hello World!";
```
- `string public greet`: Stores a public string variable initialized with **"Hello World!"**.
- The `public` modifier allows anyone to read the `greet` variable via an auto-generated getter function.

## Deployment and Usage

### Deploying the Contract
1. Use **Remix**, **Hardhat**, or **Truffle** to deploy the contract on an Ethereum-compatible network.
2. Ensure you have a Solidity compiler version `0.8.26` or compatible.

### Interacting with the Contract
- Once deployed, call the `greet` function to retrieve the stored greeting message.

### Example Usage
#### Calling `greet()`
```bash
> contract.greet()
"Hello World!"
```

## License
This project is licensed under the [MIT License](LICENSE).

