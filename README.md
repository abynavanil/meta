# Meta

This is a simple ERC-20 token contract named "MyToken" with the symbol "phundaaaaa". It has the following features:

Public variables for the token name, token abbreviation, and total supply
Mapping variable to store the balances of each address
Mint function to create new tokens and assign them to an address
Burn function to destroy tokens from an address

## Description

This smart contract implements a simple ERC-20 token named "Aniland" with the abbreviation "phundaaaaa". It allows users to mint and burn tokens.


## Getting Started

To use this contract, you will need to deploy it to a blockchain network. You can do this using a tool like Remix or Truffle. Once you have deployed the contract, you will need to interact with it using its functions. You can do this using a web3 library or a tool like Remix.

### Executing program

To execute the program, you will need to call the mint or burn functions. The mint function takes two arguments: the address to mint the tokens to and the number of tokens to mint. The burn function takes two arguments: the address to burn the tokens from and the number of tokens to burn.

```javascript
pragma solidity ^0.8.4;

  // mint function
    function mint(address _address, uint _value)public {
        totalSupply+=_value;
        balances[_address]+=_value;
    }


```

```javascript
pragma solidity ^0.8.4;

// burn function
    function burn(address _address, uint _value)public {
        if (balances[_address]>=_value){
            totalSupply-=_value;
            balances[_address]-=_value;

        }
        
    }


```

To mint tokens, call the mint function, passing the address of the recipient and the amount of tokens to mint.

To burn tokens, call the burn function, passing the address of the sender and the amount of tokens to burn.

## Authors

Abhinav Anil



## License

This project is licensed under the MIT License - see the LICENSE.md file for details
