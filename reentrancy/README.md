# Best practice
## ReentrancyGuard
- Implement a lock which protects a contract from being re-entered when calling other contract.
- [ReentrancyGuard by Open Zeppelin](https://docs.openzeppelin.com/contracts/3.x/api/utils#ReentrancyGuard)

## Checks-Effects-Interactions pattern
- Avoid state changes after external calls. [Use the Checks-Effects-Interactions Pattern](https://docs.soliditylang.org/en/v0.6.11/security-considerations.html#use-the-checks-effects-interactions-pattern).
- [SWC-107](https://swcregistry.io/docs/SWC-107)

# Previous Known Attacks
- [The DAO](https://www.coindesk.com/understanding-dao-hack-journalists)
- [Lendf.me](https://slowmist.medium.com/slowmist-details-of-lendf-me-reentrancy-attack-3e168ab5f2b1)
- [imBTC Uniswap Pool](https://defirate.com/imbtc-uniswap-hack/)

# References
- [Reentrancy After Istanbul By Open Zeppelin](https://blog.openzeppelin.com/reentrancy-after-istanbul/)
- [Reentrancy Best Practices By Consensys](https://consensys.github.io/smart-contract-best-practices/known_attacks/#reentrancy)
- [Solidity doc](https://docs.soliditylang.org/en/v0.5.11/security-considerations.html#re-entrancy)
