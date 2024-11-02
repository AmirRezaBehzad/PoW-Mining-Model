# PoW Mining Model
This repository contains a simple Proof-of-Work (PoW) mining simulation using SHA-256 hashing. The project demonstrates fundamental mining principles in blockchain technology, including nonce discovery, hash-based data integrity, and achieving target difficulty by requiring leading zeroes in the hash. This implementation helps illustrate how blockchains ensure immutability and secure data through cryptographic hashing.
## Requirements
- Python 3 (available in Google Colab)
- hashlib (included in the Python standard library)
- logging (included in the Python standard library)
## Project Overview
### Introduction
The PoW Mining Model is a Python-based project simulating the mining process by searching for a valid nonce that generates a SHA-256 hash with a specified number of leading zeroes. This Proof-of-Work approach forms the basis of blockchain networks, ensuring data integrity and preventing tampering by requiring computational effort to add new blocks.
### Key Features
1. Proof-of-Work Mining Process:
- The script iterates through nonces until it finds one that produces a hash meeting the target difficulty (six leading zeroes in this example).
2. SHA-256 Hashing:
- SHA-256 hashing secures data by producing unique, fixed-length outputs. A small change in the input data results in a significantly different hash, demonstrating the "avalanche effect."
3. Nonce Discovery:
- Nonces are incremented in search of a suitable hash. Once found, the nonce and its corresponding hash simulate how block mining works in a blockchain.
### Running in Google Colab

1. Open Google Colab:
- Go to Google Colab and create a new notebook.
2. Copy the Code:
- Copy the code from this repository and paste it into a cell in your Colab notebook.
3. Run the Cell:
- Execute the cell by pressing Shift + Enter. The code will start the mining process, displaying the nonce and final hash once a valid nonce is found.
4. Experiment with Data:
- You can modify block_number, transactions, and previous_hash values in the code cell to simulate different mining scenarios. Adjust the ZEROES constant to increase or decrease the mining difficulty.
### Avalanche Effect Demonstration
This project showcases the avalanche effect through SHA-256 hashing: even a slight change in transactions or previous_hash results in a completely different hash. This illustrates the blockchain's security, where any tampering is immediately detectable through hash inconsistencies.
### Conclusion
The PoW Mining Model provides a basic understanding of blockchain mining and Proof-of-Work. By simulating nonce discovery and cryptographic hashing, it demonstrates key blockchain principles, including data integrity, immutability, and the importance of hash functions in securing a blockchain. This project is a practical starting point for anyone interested in learning more about blockchain fundamentals.
