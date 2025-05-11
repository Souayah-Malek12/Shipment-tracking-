# Shipment Tracking dApp

 # 📦 Shipment Tracking DApp

A decentralized shipment tracking application built using **Angular** for the frontend and **Solidity smart contracts** deployed via **Truffle**.

Users can connect their wallets, create shipments, and track real-time status updates stored immutably on the blockchain.

---

## 🚀 Features

- 🔐 Wallet connection with MetaMask  
- 📦 Create new shipments with sender/receiver info  
- 🗺️ View list of all tracked shipments  
- 📄 View detailed history of each shipment  
- 🧾 Powered by secure Ethereum-based smart contract (`Shipment.sol`)

---

## 🛠 Tech Stack

| Layer       | Technology Used                     |
|-------------|-------------------------------------|
| Frontend    | Angular 18                          |
| Blockchain  | Ganache                             |
| Framework   | Truffle                             |
| Contracts   | Solidity                            |
| Web3        | Web3.js                             |
| Wallet      | MetaMask                            |

---


## 📁 Project Structure

shipment-ang/
├── client/                        # Angular frontend
│   ├── src/                       # Source files
│   │   ├── app/                   # Angular app modules and components
│   │   │   ├── base-layout/       # Layout wrapper (header/footer)
│   │   │   ├── components/        # Reusable UI components
│   │   │   │   └── shared/        # Shared components (footer, menu, top bar)
│   │   │   ├── contracts/         # Contract ABIs and addresses
│   │   │   ├── pages/             # Feature pages
│   │   │   │   ├── connect-wallet/    # Wallet connection page
│   │   │   │   ├── create-shipment/   # Create new shipment form
│   │   │   │   ├── shipment-detail/   # Shipment status details page
│   │   │   │   └── shipment-list/     # List of all tracked shipments
│   │   │   ├── app-routing.module.ts  # Routing configuration
│   │   │   ├── app.component.*        # Root component files
│   │   │   ├── app.module.ts          # AppModule definition
│   │   │   └── web3-service.service.ts# Web3 interaction service
│   │   ├── assets/                # Static assets (images, JSONs)
│   │   ├── index.html             # Main HTML entry point
│   │   ├── main.ts                # Bootstrapping file
│   │   └── styles.css             # Global styles
│   ├── node_modules/              # Installed npm packages
│   ├── public/                    # Static files served as-is
│   ├── angular.json               # Angular CLI configuration
│   ├── package-lock.json          # Dependency versions lock
│   ├── package.json               # Project metadata and scripts
│   └── README.md                  # Frontend-specific README
│
├── truffle/                       # Smart contract project
│   ├── contracts/                 # Solidity source files
│   │   └── Shipment.sol           # Core shipment tracking contract
│   ├── migrations/                # Deployment scripts
│   │   └── 2_deploy_shipment.js   # Script to deploy contract
│   ├── test/                      # Unit tests for contracts
│   └── truffle-config.js          # Network and compiler settings
│
└── README.md                      # This file – overall project overview

---

## 🚀 Getting Started

### 1. Prerequisites

- Node.js and npm
- Angular CLI (`npm install -g @angular/cli`)
- Truffle (`npm install -g truffle`)
- Ganache (GUI or CLI)
- MetaMask browser extension

---

### 2. Run Ganache

Start Ganache and create a new workspace (or run `ganache-cli` in terminal).

---

### 3. Compile & Deploy Smart Contracts

Open a terminal in the `truffle/` directory:

```bash
cd truffle
truffle compile
truffle migrate --network ganache

### 4. Install Dependencies and Start the Angular Frontend

From the root project directory, run the following commands:

```bash
cd client          # Navigate to the Angular client folder
npm install        # Install all required packages
ng serve           # Start the Angular development server

