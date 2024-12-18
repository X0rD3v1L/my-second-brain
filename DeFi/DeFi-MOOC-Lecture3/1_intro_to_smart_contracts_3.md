## Intro to Smart Contracts

#### Smart Contract Demo

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.4;

contract BellTower {
    uint public bellRung;

    event BellRung(uint rangForTheNthTime, address whoRangIt);

    function ringTheBell() public {
        bellRung++;

        emit BellRung(bellRung, msg.sender);
    }
}
```

