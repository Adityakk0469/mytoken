# My Token

This Solidity contract implements a basic ERC20-like token with mint and burn functionalities.

## Contract Overview

### The MyToken contract includes:

* Public variables for the token name, abbreviation, and total supply.
* A mapping to track the balances of different addresses.
* Functions to mint and burn tokens.

## Public Variables

* string public tokenname: The name of the token. Initialized to "Aditya Token".
* string public tokenabbrv: The abbreviation of the token. Initialized to "ADT".
* uint public totalsupply: The total supply of the tokens. Initialized to 0.

## Mapping

* mapping(address => uint) public balances: A mapping that stores the balance of each address.

  
## Getting Started

### Installing

* To run test the program just copy the content of mytoken.sol

### Executing program

* Open Remix IDE. https://remix.ethereum.org/
* Create a new file and paste the contract code.
* Compile the contract.
* Deploy the contract.
```
// SPDX-License-Identifier: MIT
pragma solidity 0.8.18;

contract MyToken {

    // public variables here
    string public tokenname="Aditya Token";
    string public tokenabbrv="ADT";
    uint public totalsupply = 0;

    // mapping variable here
    mapping(address => uint) public balances;

    // mint function
    function mint(address _address , uint _value)public{
        totalsupply += _value;
        balances[_address] += _value;
    }

    // burn function
    function burn(address _address , uint _value)public{
        if(balances[_address]>= _value){
            totalsupply -= _value;
            balances[_address] -= _value;
        }
    }

}
```



## Authors

Aditya Kumar 

