# Simple Blockchain in Python

A minimal blockchain implementation built using **Python** and **Flask**, designed to demonstrate the core principles of blockchain technology — including blocks, transactions, proof of work, and decentralized consensus.

---

## Features

* **Blockchain Structure** – Stores blocks containing transactions and hashes of previous blocks
* **Transactions** – Record sender, recipient, and amount details
* **Proof of Work (PoW)** – Simple algorithm to simulate mining and block validation
* **Node Registration** – Connect multiple nodes across the network
* **Consensus Algorithm** – Ensures all nodes share the same authoritative chain

---

## Tech Stack

* **Python 3**
* **Flask** – for RESTful APIs
* **Hashlib** – for SHA-256 hashing
* **Requests** – for node communication

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/<your-username>/simple-blockchain.git
cd simple-blockchain
```

### 2. Install Dependencies

Make sure Flask and Requests are installed:

```bash
pip install flask requests
```

### 3. Run the Blockchain Node

```bash
python blockchain.py
```

By default, the Flask server runs at:

```
http://127.0.0.1:5000
```

---

## API Endpoints

| Endpoint            | Method | Description                                |
| ------------------- | ------ | ------------------------------------------ |
| `/mine`             | GET    | Mines a new block and adds it to the chain |
| `/transactions/new` | POST   | Creates a new transaction                  |
| `/chain`            | GET    | Returns the full blockchain                |
| `/nodes/register`   | POST   | Registers new nodes to the network         |
| `/nodes/resolve`    | GET    | Runs the consensus algorithm               |

---

## Example Request

**Create a new transaction:**

```bash
POST /transactions/new
Content-Type: application/json

{
  "sender": "Alice",
  "recipient": "Bob",
  "amount": 10
}
```

---

## Learning Outcomes

Through this project, I explored:

* How blockchain data is structured and linked via cryptographic hashes
* How Proof of Work ensures computational difficulty
* How consensus keeps distributed systems consistent
* How Flask can be used to simulate decentralized communication

---

## Contributing

Feel free to fork this project, open issues, or submit pull requests.
I’d love feedback or suggestions to improve it!

---

## Author

**Dhruv**

Learning by building – exploring blockchain and decentralized systems.
