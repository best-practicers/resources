# Ownership and access control in Solidity

We define ownership audit as audit of access control within contract by owners (developers) as well as proper setting of roles in relation to access policy by owners or other contract users. Appropriate policy setting should address following issues:

1) Potential vulnerabilities resulting in funds loss due to inappropriate access control settings, e.g contract takeover.
2) Potential vulnerabilities resulting in misuse of contract functions, e.g unauthorized withdraw.
3) Risks to user funds by malicious developers, e.g 'rug pulls' or 'yanking' of user wallet funds by, for example, infinite approve.
4) Management of owner keys, e.g Openzeppelin Defender framework.

## Methods of access control

1) Ownable.sol (Simple)
2) Whitelisting (Medium)
3) RBAC (Complex)

Source: [Guide to ownership and access control in solidity](https://medium.com/coinmonks/guide-to-ownership-and-access-control-in-solidity-f2d99f63c6d4)

## Resources

Most basic access control scenarios can currently be found in Openzeppelin library

[Openzeppelin Access Control library](https://docs.openzeppelin.com/contracts/2.x/access-control)

3000 feet view of what exactly is access control

[Access restriction](https://fravoll.github.io/solidity-patterns/access_restriction.html
)

[Advanced role based access control in practice](https://hiddentao.com/archives/2020/03/21/advanced-role-based-access-control-in-solidity
)

### Real world examples

[Dasp.co](https://dasp.co/#item-2
)

[Vulnerable contracts by example](https://github.com/smartbugs/smartbugs/tree/master/dataset/access_control
)

## RBAC - Complex policy control


[Multi-Authority Attribute-Based Access Control with Smart Contract](https://arxiv.org/pdf/1903.07009.pdf)

[Dynamic Role-Based Access Control for Decentralized Applications](https://arxiv.org/pdf/2002.05547.pdf)

