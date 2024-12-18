## Intro to Smart Contracts

#### Gas in Ethereum

> Each transaction has to pay a gas fee

More complicated transactions pay more gas fee.

The more gas you pay the more faster the transaction executes.

Miners limited by a global limit on gas per block.

> Every instruction consumes a fixed amount of gas

A counter of gas used is tracked when executing the transaction.

> Gas limits and refunds

- Each transaction specifies a gas limit and a price for the gas, in units of ether.
- Ether value to pay for the gas need to paid upfront
- At the end of the contract, unused gas is refunded.

> Gas Prices per opcode

Gas price is determined based on the compiled opcodes for EVM, not high level code.

> What happens when gas runs out?

- An **Out of Gas** exception is thrown
- Any changes made to the storage variables, any account transfers, are reverted to their state before the method call.
- You are still charged the gas fee for every instruction leading up to this exception.
