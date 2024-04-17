**SupplyChain-Dapp: Blockchain-Based Pharmaceutical Supply Chain Management**

This DApp implements transparent and secure supply chain management using blockchain technology. 

**Key Features:**

* **Smart Contract Management:** Tracks product movement from manufacturer to customer.
* **Ethereum Development Environment:** Utilizes Truffle.js, Ganache, and the Geode Testnet.
* **Frontend:** Web3.js for smart contract interaction.
* **MetaMask Integration:** Connects wallets to the Geode Testnet for transactions.

**🔧 Setting up Local Development**

**1. Prerequisites**

* Node.js ([https://nodejs.org/](https://nodejs.org/))
* Git ([https://git-scm.com/downloads](https://git-scm.com/downloads))
* VS Code ([https://code.visualstudio.com/](https://code.visualstudio.com/))
* Ganache ([https://www.trufflesuite.com/ganache](https://www.trufflesuite.com/ganache))
* MetaMask browser extension

**2. Project Setup**

* Clone the repository:
   ```bash
   git clone https://github.com/Roshanlj/Pharma-Supply-Chain
   ```
* Install dependencies:
   ```bash
   cd Pharma-Supply-Chain
   npm i
   ```

**3. Smart Contract Deployment**

* Compile contracts:
   ```bash
   truffle compile
   ```
* Start Ganache (get RPC server URL)
* Update `truffle-config.js` with Ganache RPC details.
* Deploy contracts:
   ```bash
   truffle migrate
   ```

**4. Run the DApp**

* In a separate terminal, navigate to the 'client' directory:
   ```bash
   cd client
   ```
* Install frontend dependencies: 
   ```bash
   npm i 
   ```
* Start the development server:
   ```bash
   npm start
   ```

**5. Connect MetaMask**

* Add Ganache as a custom network in MetaMask using the RPC server URL.
* Import Ganache accounts into MetaMask for testing.

**Let me know if you'd like any additional adjustments or have specific formatting requirements!** 
