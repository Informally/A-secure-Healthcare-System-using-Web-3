Here’s the full `README.md` content you can copy and paste directly into your file:

```markdown
# Nurse Dashboard Healthcare System

This project is a web-based healthcare system for nurses to manage patient medical records and add remarks. It uses a blockchain-based smart contract to securely store patient data and remarks. The application runs locally using `lite-server`.

---

## Features

- View registered patients and their medical records.
- Add and edit patient medical records.
- Request Connection between Patient and Doctors.
- Secure interaction with the blockchain via MetaMask.
- Live reload during development using `lite-server`.

---

## Prerequisites

To run the system, you need:

- [Node.js](https://nodejs.org/) installed.
- MetaMask browser extension installed and configured.
- [Ganache](https://trufflesuite.com/ganache/) installed for local Ethereum blockchain.
- `lite-server` installed (as part of the project dependencies).
- Access to Remix IDE for deploying the smart contract.

---

## Installation and Setup

### Step 1: Clone the Repository

Clone this repository to your local machine:

```bash
git clone https://github.com/<your-username>/<repository-name>.git
```

Replace `<your-username>` and `<repository-name>` with the appropriate values.

---

### Step 2: Navigate to the Project Directory

Move into the project folder:

```bash
cd <repository-name>
```

---

### Step 3: Install Dependencies

Install the required dependencies using:

```bash
npm install
```

---

### Step 4: Start the Local Blockchain (Ganache)

1. Open Ganache and create a new workspace or use the Quickstart Ethereum option.
2. Copy the RPC server URL (e.g., http://127.0.0.1:7545) and configure MetaMask to connect to this local blockchain:
    -Open MetaMask and go to Settings > Networks.
    -Add a new network with the following details:
            -Network Name: Ganache
            -RPC URL: http://127.0.0.1:7545
            -Chain ID: 1337
            -Currency Symbol: ETH
3. Import one of the private keys provided by Ganache into MetaMask.

### Step 5: Start the Server

Run the application locally using:

```bash
npm start
```

This will start the application and serve it at:

```
http://localhost:3000
```

Open your browser and navigate to this URL.

---

## Deploying the Smart Contract

### Step 1: Open Remix IDE

Go to [Remix IDE](https://remix.ethereum.org/).

---

### Step 2: Add the Smart Contract

Copy the smart contract code in Contracts Folder (Agent.sol) and paste it into a new file (e.g., `Agent.sol`) in Remix.

---

### Step 3: Compile the Contract

- Select the appropriate Solidity version matching your smart contract.
- Click "Compile" to compile the contract.

---

### Step 4: Deploy the Contract

- Go to the "Deploy & Run Transactions" tab.
- Set the environment to "Injected Web3" to connect with MetaMask.
- Deploy the contract.
- Copy the deployed contract address.

---

### Step 5: Update Contract Address

Replace the placeholder contract address in the `src/js/contractConfig.js` file with the new deployed address.

---

## Folder Structure

Here’s the structure of the project:

```
Healthcare/
├── src/
│   ├── css/
│   │   └── bootstrap.min.css
│   ├── js/
│   │   ├── bootstrap.min.js
│   │   ├── contractConfig.js
│   │   └── utils.js
│   ├── nurse.html
│   └── index.html
├── package.json
├── README.md
└── ...
```

---

## Running the System Locally

- This project uses `lite-server` for local development.
- The `lite-server` serves the `src` folder at `http://localhost:3000` and automatically reloads changes.
- To start the server, use:

```bash
npm start
```

---

## Troubleshooting

### Issue: Missing Files (404 Errors)
- Ensure that required files (e.g., `bootstrap.min.js`, `contractConfig.js`) exist in the correct directories.
- Reinstall missing dependencies, if necessary:

```bash
npm install bootstrap
```

### Issue: Unable to Interact with Blockchain
- Ensure MetaMask is connected to the same network as the smart contract.
- Verify the `contractConfig.js` file contains the correct contract address and ABI.

---

## License

This project is licensed under the MIT License.
```

Copy this into a file named `README.md`, replacing placeholders like `<your-username>` and `<repository-name>` as appropriate for your GitHub repository.
