# diamond-assembly
Diamond EIP ERC-2535 Done in EVM assembly opcodes.

The following are two different implementations of the Diamond standard EIP-2535. They are done using Trim and converted into solidity files for block exploraer compatibility. Tests are using Foundry. 

> Versions:
- [v1 - With facet array Storage address mask (Safer but slightly more gas)](https://github.com/Priceless-Tokens/diamond-assembly-v1)
- [v2 - Facet array is at start of EVM Storage. Warning. (This can be super dangerous if any storage variables do not have a set storage location. A storage collision could occur.)](https://github.com/Priceless-Tokens/diamond-assembly-v2)

> Objectives
0. Maintain security.
1. Minimize cryptocurrency user gas.
2. Compatibility with Solidity, Yul, and Fe.
3. Keep deployment and upgrades gas low as possible, while doing so trustlessly.
4. Maximize compatibility with block explorers.

> Credits:
@ 0xKitsune - https://github.com/0xKitsune/Foundry-Vyper - Modded their work on using FFI to run tests with Vyper to Trim
