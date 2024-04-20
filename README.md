## Module 1 - Blockchain Creation

This module details the implementation of a simple blockchain using Python and Flask. Below are the main components and functionalities encapsulated within this blockchain system.

### Dependencies:
- **Flask 0.12.2:** A micro web framework for Python, used to create and handle web application routes.
- **Postman HTTP Client:** A tool to interact with the web API during development.

### Features:

#### Blockchain Basics:
- **Class Definition:** Defines a `Blockchain` class that encapsulates all the blockchain operations.
- **Block Creation:** Each block contains an index, timestamp, cryptographic hash of the previous block, proof of work, and list of transactions.
- **Genesis Block:** Automatically creates the first block of the blockchain with predefined values.

#### Proof of Work:
- Implements a proof of work algorithm to secure the blockchain and prevent tampering, ensuring that creating new blocks requires computational effort.

#### Chain Validation:
- Validates the integrity of the entire blockchain, ensuring the chain's hashes and proofs are consistent.

#### Transaction Handling:
- Supports adding transactions to the blockchain, which will be included in the next mined block.

#### Blockchain Network:
- Adds functionality to connect multiple nodes in the blockchain network.
- Ensures the network's consistency by replacing the local chain with the longest chain found across the network.

### Web API:
Utilizes Flask to create a web application that allows interaction with the blockchain through HTTP requests.
- **Mining Blocks:** A route to mine a new block and receive rewards.
- **Querying the Full Chain:** A route to retrieve the entire blockchain.
- **Chain Validity:** A route to check if the blockchain is valid.
- **Transaction Addition:** A route to add new transactions.
- **Node Connection:** A route to connect new nodes to the blockchain network.
- **Chain Replacement:** A route to replace the local chain with the longest one in the network.

### Running the Application:
The application runs on `host = '0.0.0.0'` and `port = 5000`, making it accessible from any device within the network.

This module demonstrates the foundational concepts of a blockchain system and allows for further expansion into a more robust, decentralized blockchain network.
