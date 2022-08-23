# diamond-assembly
Diamond EIP ERC-2535 Done in EVM assembly opcodes.

The following are two different implementations of the Diamond standard EIP-2535. They are done using Trim and converted into solidity files for block exploraer compatibility.

> Versions:
- v1 - With facet array Storage address mask (Safer but slightly more gas)
- v2 - Facet array is at start of EVM Storage. Warning. (This can be super dangerous if any storage variables do not have a set storage location. A storage collision could occur.) 
