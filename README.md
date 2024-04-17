## Description
Supply chain is always hard to manage and requires a lot of admistrative machinery. However, when managed with smart contracts using blockchain, a lot of the paperwork is reduced.
Also it leads to an increase in the transparency and helps to build an efficient Root of Trust. Supply-chain-dapp is such an implementation of a supply chain management system which uses blockchain to ensure a transparent and secure transfer of product from the manufacturer to the customer via the online e-commerce websites. 
## Architecture
The smart contract is being written with Solidity which is then compiled, migrated and deployed using Truffle.js on the Gode Testnet blockchain network.The frontend uses Web3.js to communicate with the smart contract and Gode Testnet blockchain network and Meta Musk Wallet is connect to Gode Test Network to do Transaction between each component in Supply .
****
![https://raw.githubusercontent.com/faizack619/Supply-Chain-Gode-Blockchain/master/client/public/Blank%20diagram.png](https://raw.githubusercontent.com/faizack619/Supply-Chain-Gode-Blockchain/master/client/public/Blank%20diagram.png)

## Supply Chain Flow


![[https://cdn.vectorstock.com/i/1000x1000/35/51/diagram-of-supply-chain-management-vector-41743551.webp](https://cdn.vectorstock.com/i/1000x1000/35/51/diagram-of-supply-chain-management-vector-41743551.webp)](https://cdn-wordpress-info.futurelearn.com/info/wp-content/uploads/8d54ad89-e86f-4d7c-8208-74455976a4a9-2-768x489.png)



## Smart Contract Working Flow

![https://raw.githubusercontent.com/faizack619/Supply-Chain-Gode-Blockchain/master/client/public/Supply%20Chain%20Design%20(1).png?token=GHSAT0AAAAAAB52SPAT5YHI3AALNPFXL27AY7OU3IQ](https://raw.githubusercontent.com/faizack619/Supply-Chain-Gode-Blockchain/master/client/public/Supply%20Chain%20Design%20(1).png?token=GHSAT0AAAAAAB52SPAT5YHI3AALNPFXL27AY7OU3IQ)

This is a SupplyChain smart contract written in Solidity. The contract models the various roles and stages involved in the supply chain of a pharmaceutical product.

The contract owner is the person who deploys the contract and is the only one who can authorize various roles like retailer, manufacturer, etc.

There are several roles involved in the supply chain of the pharmaceutical product. These include the raw material supplier, manufacturer, distributor, and retailer.

The smart contract stores information about the medicine, such as its name, description, and current stage in the supply chain. There is also a function to show the current stage of a medicine, which can be used by client applications.

The smart contract also stores information about the various players in the supply chain, such as their name, address, and place of operation.

The addRMS(), addManufacturer(), addDistributor(), and addRetailer() functions can be used by the contract owner to add new players to the supply chain.

Overall, this smart contract provides a way to track the various stages of a pharmaceutical product in the supply chain, ensuring transparency and accountability.


##  🔧 Setting up Local Development

### Step1.
## Installation and Setup

* **VSCODE** : VSCode can be downloaded from https://code.visualstudio.com/
* **Node.js** : Download the latest version of Node.js from https://nodejs.org/ and after installation check     Version using terimal: node -v .
* **Git** : Download the latest version of Git from the official website at https://git-scm.com/downloads and   check Version using terimal: git --version.

* **Ganache** : Download the latest version of Ganache from the official website at https://www.trufflesuite.com/ganache.
* **MetaMask** : can be installed as a browser extension from the Chrome Web Store or Firefox Add-ons store.
  
### Step2.
## Create,Compile & Deploy Smart Contract. 

* Open VScode and open VScode Terimal by Ctrl + ' .
* **Clone Project** Type the following command and press Enter : git clone : ` https://github.com/faizack619/Supply-Chain-Blockchain.git  
* **Install truffle** : Type the following command and press Enter: `npm install -g truffle`
* **Install dependencies** : Type the following command and press Enter: `npm i`
* **File structure for  DApp** : 
  
    **contracts**: This folder contains the Solidity smart contracts for the DApp. The Migrations.sol contract is automatically created by Truffle and is used for managing migrations.

    **migrations**: This folder contains the JavaScript migration files used to deploy the smart contracts to the blockchain network.

    **test**: This folder contains the JavaScript test files used to test the smart contracts.

    **truffle-config.js**: This file contains the configuration for the Truffle project, including the blockchain network to be used and any necessary settings.

    **package.jso**n: This file contains information about the dependencies and scripts used in the project.

    **package-lock.json**: This file is generated automatically and contains the exact version of each dependency used in the project.

    **Client**s: This Folder contains the client-side code, typically HTML, CSS, and JavaScript, can be organized into a client folder.
* **Compile the smart contract** :  In the terminal, use the following command to compile the smart contract: `truffle compile` 
* **Deploy the smart contract** :
   
    * After Compile We Need To Deploy Your Smart Contract on Blockchain. In Our Case We are Using Ganache Which is personal blockchain for Ethereum development, used to test and develop Smart Contracts.

    * Open Ganache and create new WorkSpace.Copy Rpc Server Address.

    * ![https://miro.medium.com/max/1248/1*4rzNT0muOXelP22Ky9178g.png](https://miro.medium.com/max/1248/1*4rzNT0muOXelP22Ky9178g.png)

    * The RPC server is used to allow applications to communicate with the Ethereum blockchain and execute smart contract transactions, query the state of the blockchain, and interact with the Ethereum network.

    * Now to add Rcp address in our truffle-config.js and the replace host address and port address with Our Ganache Rcp.

    * ![https://developers.rsk.co/assets/img/tutorials/truffle-test/image-04.png](https://developers.rsk.co/assets/img/tutorials/truffle-test/image-04.png)
  
    * After Changing RCP address.Open terminal and run this cmd : `truffle migrate`.
    * This Command Will deploye Smart Contract to Blockchain.

### Step 3.
## Run DAPP. 
* Open a second terminal and enter the client folder
  * `cd client`
 
* Install all packages in the package.json file
  * `npm i`
  
* Install Web3 in the package.json file
  * `npm install -save web3`


* Run this Command :
  * `npm`
 
* Run the app 
  * `npm start`

* The app gets hosted by default at port 3000.

### Step 4.
## Connect Meta Musk with Ganache. 

1. Start Ganache: Start the Ganache application and make note of the RPC server URL and port number.

1. Connect MetaMask: Open MetaMask in your browser and click on the network dropdown in the top-right corner.

Select "Custom RPC" and enter the RPC server URL and port number for your Ganache instance. Click "Save".

1. Import an account: In Ganache, click on the "Accounts" tab and select the first account listed. Click on the "Copy" button next to the "Private Key" field copy the private key.

 2. In MetaMask, click on the three dots in the top-right corner, select "Import Account", and paste the private key into the private key field. Click "Import".

 3. Add All participate(Raw Material,Supplier,Manufacture,Retail). by following above Step

