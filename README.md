# Solidity Owner View

https://sepolia.etherscan.io/address/0x8207ba6852ee561f0786e2d876b1a20fef916e46

```solidity
// SPDX-License-Identifier: MIT
pragma solidity 0.8.18;

contract OnlyOwner {

    function getNum() public view returns(uint) {
        require(msg.sender == 0xdD4c825203f97984e7867F11eeCc813A036089D1, "onnly onwer can view");
        return 123;
    }

}
```