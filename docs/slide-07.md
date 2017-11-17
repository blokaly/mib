## Eethereum &ETH;App

[https://www.stateofthedapps.com/whats-a-dapp](https://www.stateofthedapps.com/whats-a-dapp)

- A &ETH;App is a Decentralized Application
- Traditional Web Application on the front-end
- Ethereum (Blockchain) on the back-end

---

## High Level Overview

![](images/dapp-overview.png)

(https://medium.com/@mvmurthy/ethereum-for-web-developers-890be23d1d0c)

---

## DAO

- **D**ecentralized **A**utonomous **O**rganization
- Organization run through rules encoded by smart contracts
- Issues

---

## Examples

- https://www.stateofthedapps.com/
- https://www.zastrin.com/simple-ethereum-voting-dapp.html

[Ropsten Testnet Faucet](https://ethtools.com/ropsten/tools/faucet/)

---

## Solidity

[http://solidity.readthedocs.io/en/latest/](http://solidity.readthedocs.io/en/latest/)

```json
pragma solidity ^0.4.11;

contract Ballot {
    struct Voter {
        uint weight;
        bool voted;
        address delegate;
        uint vote;
    }

    address public chairperson;

    mapping(address => Voter) public voters;

    Proposal[] public proposals;
}    
```