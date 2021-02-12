# testing

Testing is a necessary activity in software development. When developing smart contracts testing assumes an even greater role as SC are usually immutable so it is not possible to fix them after deployment. Besides its primary role of asserting precondions and invariants, testing is also a very useful tool during development to clarify hidden assumptions and have a better understanding of what the software is supposed to do. 

## Types of testing
Testing happens at different level of abstractions and achieves different goals. Different levels of testing have different levels of automation. 

### Unit testing
Unit testing is genereally used at a single module level (function or contract), the main goal is to assure internal quality. These are the most numerous tests and we use them to assert invariants and to assure edge cases are properly managed by our software.
If needed, at this testing levels, dependecies are mocked.

### Integration testing
Integrations testing is used to validate the communication protocol between multiple modules, we mainly test API interactions. This can go from something as simple as the interaction between two smart contracts to a full blown project to project testing. At this level some dependecies can be mocked.

#### Forked mainnet testing
A subset of integration testing is forked mainnet testing. This type of test is used to replicate conditions close the productive environment. In some cases this type of test is the only way to test large interactions between multiple projects as some projects are only deployed in mainnet.
The way this type of test operates is by snapshotting the blockchain at a specific block and allowing us to manipulate it via our smart contracts and/or special evm operations (e.g. impersonate account)

### Manual QA
Manual QA can be performed locally, in testnet, or in mainnet. This type of test usually consists of speculative test which might enact scenarios not covered by the other type of tests.

## Tooling

### Waffle

[Waffle](https://ethereum-waffle.readthedocs.io/en/latest/) is a toolkit for modern smart contract testing. 
Highlights are:
- Smart contract mocking
- Special purpose matchers (event emitted, function called, etc)

### Hardhat

[Hardhat](https://hardhat.org/) is a smart contract development automation toolkit.
In the context of testing the main features are:
- [Mainnet forking](https://hardhat.org/guides/mainnet-forking.html)
- [Waffle Integration](https://hardhat.org/plugins/nomiclabs-hardhat-waffle.html)

## Examples

[Mainframe HQ](https://github.com/hifi-finance/hifi-protocol/tree/main/test)
