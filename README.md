# BlockBase - Expense Tracker dApp

A decentralized expense tracker built using **React**, **Solidity**, and **CSS**, allowing users to track shared expenses on the Ethereum blockchain using the Sepolia testnet.

## 🚀 Overview

This project helps you track and split expenses among participants by leveraging Ethereum smart contracts. It consists of:

- **React**: Frontend framework
- **Solidity**: Smart contract for on-chain functionality
- **CSS**: Styling (optional to modify)

![Alt text](https://github.com/sowave06/Expense_TrackerApp/blob/main/%7B3BEDBC8C-9399-4289-A676-7FE698ED2AE7%7D.png)


## 📁 Project Links

- [Smart Contract Code](https://drive.google.com/file/d/1k-6iEU_t9N0nUZYGleKm1_tq1KEcM-Xt/view?usp=share_link)
- [React Code](https://drive.google.com/file/d/1GUq_QGXZEJ13SC28TAFVBFHYJrNQqk0K/view?usp=share_link)
- [CSS File](https://drive.google.com/file/d/1SjbwH6tnLY1ppepZiJqlnT8xCt021-mr/view?usp=share_link)
- [ABI File](https://drive.google.com/file/d/1jePTtpOWQ30rOHb2e7fm6Nt_PWqHu82P/view?usp=share_link)

> 💡 Understanding the CSS is optional. ABI is provided for ease of integration.

---

## 🧰 Prerequisites

Before running the project, ensure the following are set up:

1. [Node.js and npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
2. MetaMask extension (Chrome/Firefox)
3. Sepolia Testnet ETH (Get it from a [Sepolia faucet](https://sepoliafaucet.com))

---
## Updated Feature

  Get Your Own Name
  -Allows a user to retrieve their registered name using their wallet address.
```solidity
function getYourName() public view returns (string memory) {
    require(
        people[msg.sender].walletAddress != address(0),
        "User not registered"
    );
    return people[msg.sender].name;
}
```

---

