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


## 🧠 Design Patterns:

1- Inheritance and Interfaces (Importing and extending contracts and/or using contract interfaces) Inheritances and Interfaces:
import ownable  بتاع openzeppelin

2- Access Control Design Patterns (Restricting access to certain functions using things like Ownable, Role-based Control) Access Control Design Patterns


## 🔐 Security practices:

1- Using Specific Compiler Pragma
2- Proper Use of Require
3- Proper use of .call and .delegateCall

## 🔗 Important Links & Addresses

### 📝 Smart Contract Addresses on Scroll Sepolia Testnet

- **Contract Address:** 0x5c1fE1e2c7a4A8F40B053b541a1e3B0ee5daf6Bf

### 🧾 Verified Contract on Scroll Sepolia Explorer

- **Explorer Link:** https://sepolia.scrollscan.com/address/0x5c1fE1e2c7a4A8F40B053b541a1e3B0ee5daf6Bf

### 🌐 Frontend DApp Hosting Link

- **Live DApp:** :http://193-168-175-22.cloud-xip.com/

---

## 🧪 How to Run Tests

1. 
* cd smart_contract
* Installez les dépendances :
npm install
* Exécutez les tests avec Foundry:
forge test

✅ Les tests sont situés dans le répertoire smart_contract/test/

🚀 How to Run the Program
🖥️ Run on Local Server
Naviguez vers le répertoire Dapp_Front_End/ :
cd Dapp_Front_End
Installez les dépendances : npm install
Démarrez le serveur de développement : npm run dev
L'application sera accessible à l'adresse http://localhost:3000/.

🛠️ Setting Up .env File
Créez un fichier .env dans le répertoire Dapp_Front_End/ avec le contenu suivant :

NEXT_PUBLIC_PROJECT_ID= Your_project_ID
NEXT_PUBLIC_CONTRACT_ADDRESS=0xYourContractAddressHere

⚠️ Assurez-vous de ne pas commettre votre fichier .env dans le contrôle de version.

🎥 Demo
📹 Watch the Full Walkthrough
DApp Demo Video

La démonstration couvre :

Le lancement de l'application en local

La connexion avec MetaMask

L'interaction avec le contrat intelligent (envoi de transactions)

La vérification des transactions sur Scroll Sepolia Explorer

La mise à jour en temps réel de l'interface utilisateur reflétant l'état du contrat

