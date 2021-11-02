
<h1 align="center">ERC20 Token</h1>

<div align="center">

[![Status](https://img.shields.io/badge/status-active-success.svg)]()
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](/LICENSE)

</div>

---

<p align="center"> An ERC20 Token based on OpenZeppelin contracts
    <br> 
</p>

## 📝 Table of Contents

- [About](#about)
- [Getting Started](#getting_started)
- [Configuring Your Token](#configuring)
- [Usage](#usage)
- [Deployment](#deployment)
- [Built Using](#built_using)
- [Authors](#authors)
- [Acknowledgments](#acknowledgement)

## 🧐 About <a name = "about"></a>

An ERC20 Token that is mintable, burnable, and has a max supply of 21M tokens. The premint is set at 1M tokens.
This project was made possible using openzeppelin contracts.

## 🏁 Getting Started <a name = "getting_started"></a>

### Remix IDE
Go to http://remix.ethereum.org and create a new workspace.
Under the folder contracts, create a file called "MyToken.sol" and import the code 

## 🔧 Configuring Your Token <a name = "configuring"></a>

### Set Max Supply

Set the max supply of your token by modifying the variable _maxSupply on line 20
```
    uint256 private _maxSupply = 21000000 * 10 ** decimals();
```
The max supply is set at 21000000 (21M) coins, change this accordingly to fit your needs. The max supply of tokens will never change after deployment as it will be hard-coded into the contract.

### Name Your Coin

Change the name of your token by going to line 22 and changing the text inside the quotation.

```
    constructor() ERC20("Maharmeh", "MRM") {
```
The first quotation "Maharmeh" is the coin name. The second quotation "MRM" is the symbol of the coin. Change these according to your needs.

### PreMint Amount

Change the premint amount by going to line 26 and changing the number
```
     _mint(msg.sender, 1000000 * 10 ** decimals());
```
Change 1000000 to however many tokens you would like to premint when the contract is deployed. This function is only ran once at deployment. Make sure this doesn't exceed the max supply.

## 🎈 Usage <a name="usage"></a>

Compile the code on Remix IDE using the 0.8.2 Solidity Compiler.

## 🚀 Deployment <a name = "deployment"></a>

Deploy your contract using Remix IDE. Ensure you have enough for gas fees and that you are connected to the correct network.

## ⛏️ Built Using <a name = "built_using"></a>

- [Remix](https://remix.ethereum.org) - IDE
- [OpenZeppelin](https://openzeppelin.com/) - Reusable Smart Contracts
- [Solidity](https://soliditylang.org/) - Programming Langauge

## ✍️ Authors <a name = "authors"></a>

- [@AhmadMaharmeh](https://github.com/AhmadMaharmeh) - Idea & Initial work

## 🎉 Acknowledgements <a name = "acknowledgement"></a>

- OpenZeppelin Team
