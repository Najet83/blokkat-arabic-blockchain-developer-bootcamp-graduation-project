# 🎓 Blokkat Arabic Blockchain Developer Bootcamp – Graduation Project

## 📌 About This Project

### 🔹 Project Description

This project is a decentralized application (DApp) developed as part of the Blokkat Arabic Blockchain Developer Bootcamp. It allows users to interact with a smart contract deployed on the Scroll Sepolia test network, offering features such as connect to a network via MetaMask, display wallet's balance, deposit ether, withdraw ether, display user's balance in the contract

### 🔹 Directory Structure

Dapp_Front_End
├── .env
├── README.md
├── app
│   ├── favicon.ico
│   ├── globals.css
│   ├── layout.tsx
│   └── page.tsx
├── components
│   ├── ConnectComponent.tsx
│   ├── DepositComponent.tsx
│   ├── ReadFromContract.tsx
│   └── WithdrawComponent.tsx
├── config
│   └── index.tsx
├── context
│   └── index.tsx
├── hooks
│   ├── connect.ts
│   ├── readBalance.ts
│   ├── useDeposit.ts
│   └── useWithdraw.ts
├── next-env.d.ts
├── next.config.ts
├── package-lock.json
├── package.json
├── postcss.config.mjs
├── public
│   ├── file.svg
│   ├── globe.svg
│   ├── next.svg
│   ├── vercel.svg
│   └── window.svg
└── tsconfig.json

Smart_Contract
├── .env        
├── .env.example
├── README.md   
├── foundry.toml
├── lib
│   ├── forge-std
│   └── openzeppelin-contracts
├── src
│   └── FinalProject.sol
└── test
    └── FinalProject.t.sol


## 🧠 Design Patterns

1. **Inheritance and Interfaces**  
   Import OpenZeppelin Ownable contract.  
   _Example:_ `import "@openzeppelin/contracts/access/Ownable.sol";`

2. **Access Control Design Patterns**  
   Restricting access to certain functions using Ownable.  
   _Example:_ `function withdraw(uint256 amount) external onlyOwner {...}`

3. **Optimizing Gas**  
   Using mapping instead of array.  
   _Example:_ `mapping(address => uint256) public balanceOf;`
   
## 🔐 Security practices:

1. **Using Specific Compiler Pragma**   
    _Example:_ pragma solidity 0.8.24;

2. **Proper Use of Require**   
    _Example:_ require(msg.value > 0, "You must send some ether");

3. **Proper use of .call and .delegateCall**   
    _Example:_ (bool sent, ) = msg.sender.call{value: amount}("");

## 🔗 Important Links & Addresses
### 📝 Smart Contract Addresses on Scroll Sepolia Testnet

- **Contract Address:** 0x5c1fE1e2c7a4A8F40B053b541a1e3B0ee5daf6Bf

### 🧾 Verified Contract on Scroll Sepolia Explorer

- **Explorer Link:** https://sepolia.scrollscan.com/address/0x5c1fE1e2c7a4A8F40B053b541a1e3B0ee5daf6Bf

### 🌐 Frontend DApp Hosting Link

- **Live DApp:** :http://193-168-175-22.cloud-xip.com/

## 🧪 How to Run Tests

1. Navigate to the frontend directory:    
    cd smart_contract
2. Install dependencies :   
    npm install
3. Execute tests with Foundry:   
    forge test

✅ the test file "FinalProject.t.sol" is located in the test directory inside the smart_contract folder. (smart_contract/test) 
These tests cover the core functionalities of the smart contract.

🚀 How to Run the Program

🖥️ Run on Local Server

1. Navigate to the frontend directory:  
    cd Dapp_Front_End
2. Install the dependencies:  
    npm install
3. Start the development server:  
    npm run dev
4. The application will be available at:  
    http://localhost:3000/

🛠️ Setting Up .env File

1. Create a .env file by copying the provided example:   
    cp .env.example .env
2. Open the .env file and replace the placeholder values with your actual configuration.   
    _Example:_    
       NEXT_PUBLIC_PROJECT_ID= Your_project_ID         
       NEXT_PUBLIC_CONTRACT_ADDRESS=0xYourContractAddressHere    


⚠️ Warning: Never commit your .env file to version control. It may contain sensitive information such as API keys or contract addresses. Use .env.example instead to document required variables.

🎥 Demo
📹 Watch the full walkthrough of the DApp in action:

📺 Demo Video Link ← (replace with your actual video link)

The demo includes:

* Connecting MetaMask wallet

* Submitting transactions from the frontend

* Viewing on-chain data updates

* Checking the transaction on ScrollScan

