# Lesson 2: Storage Factory

View the smart contract's creation on the test (Rinkeby's) Etherscan: https://rinkeby.etherscan.io/address/0x10aad0e4f373948465a0928d7b77cbfc0ecb577c

We discuss the Factory pattern. What is Factory pattern?

You can have multiple contracts in the same file.

You import another contract using the code below:
// SPDX-License-Identifier: MIT
pragma solidity ^0.6.0;
import "./SimpleStorage.sol";


Inheritance in Solidity is done this way: 
contract StorageFactory is SimpleStorage {
}
