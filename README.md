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
code blocks for commands
```

## Help

Any advise for common problems or issues.
```
command to run if program contains helper info
```

## Authors

Contributors names and contact info

ex. Dominique Pizzie  
ex. [@DomPizzie](https://twitter.com/dompizzie)


## License

This project is licensed under the [NAME HERE] License - see the LICENSE.md file for details
