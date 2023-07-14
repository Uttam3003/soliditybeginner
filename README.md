# Solidity Beginner
# MyToken
MyToken is a Solidity contract that represents a custom token called "META" (MTA). 
The contract allows for the minting and burning of tokens, as well as maintaining balances for different addresses.

## Token Details
### The token has the following details:

Name: META
Abbreviation: MTA
Public Variables
The contract defines the following public variables:

### TokenName: A string variable that stores the name of the token ("META").
### TokenAbbrv: A string variable that stores the abbreviation of the token ("MTA").
### TotalSupply: An unsigned integer variable that stores the total supply of the token.It is initialized to 0.
Balances Mapping
The contract uses a mapping named balances to associate addresses with their respective token balances. 
It maps addresses to unsigned integer values representing the token balance of each address.

## Mint Function
The contract provides a mint function that allows for the creation of new tokens. The function takes two parameters: an address and a value. 
The function increases the total supply of tokens by the specified value and adds the same value to the balance of the provided address.

## Burn Function
The contract also provides a burn function, which allows for the destruction of tokens. Similar to the mint function, it takes an address and a value as parameters. 
The function deducts the specified value from the total supply and from the balance of the given address.

The burn function includes a conditional statement to ensure that the balance of the address is greater than or equal to the amount that is supposed to be burned. 
If the condition is met, the function reduces the total supply and the address balance accordingly.

Please note that this implementation does not include any additional features such as transfer functions or any functionality related to token transfers between addresses. 
It focuses solely on the minting and burning of tokens.

## License
This contract is licensed under the GNU General Public License v3.0. For more information, see the (LICENSE) file.
