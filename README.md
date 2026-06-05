# Blockchain-Based File Sharing System

## Overview

The **Blockchain-Based File Sharing System** is a decentralized peer-to-peer file sharing platform that leverages blockchain technology to ensure security, transparency, and decentralization during file transfer operations.

The system combines **Blockchain**, **IPFS (InterPlanetary File System)**, **AES Encryption**, **SHA-256 Hashing**, and **Peer-to-Peer Networking** to securely share files between authorized users while maintaining file integrity and privacy.

---

# Developed By

## Daksh Bhasin

GitHub: https://github.com/dakshiitd

---

# Project Objective

The objective of this project is to create a secure decentralized file-sharing ecosystem where:

* Files are shared peer-to-peer
* Blockchain ensures immutability
* IPFS provides decentralized storage
* AES encryption protects file contents
* SHA-256 ensures integrity verification
* Socket programming enables decentralized networking

---

# Features

* Peer-to-peer decentralized file sharing
* Permissioned blockchain network
* AES encrypted file uploads
* SHA-256 file integrity validation
* IPFS decentralized storage
* Blockchain-based metadata storage
* Secure file key mechanism
* Node synchronization through sockets
* Upload and download using hash verification
* Lightweight blockchain architecture

---

# Technology Stack

## Backend

* Python
* Socket Programming
* Blockchain Architecture

## Decentralized Storage

* IPFS

## Security

* AES Encryption
* SHA-256 Hashing

## Networking

* Peer-to-Peer Network
* Permissioned Blockchain

---

# System Architecture

The system architecture contains:

```text
User Upload
    ↓
AES Encryption
    ↓
IPFS Storage
    ↓
Generated File Hash
    ↓
Blockchain Storage
    ↓
P2P Network Synchronization
    ↓
Receiver Downloads File
    ↓
AES Decryption
```

---

# Methodology

## 1. Creating the Blockchain

### Block Structure

Each block consists of:

### Block Number

Represents block index.

* Block 0 → Genesis Block

### Timestamp

Stores creation time of block.

### Proof (Nonce)

Used for mining and generating valid hashes.

### Previous Hash

Links previous blocks together.

### Sender

Identity of uploader.

### Receiver

Intended recipient.

### File Hash

Hash returned from IPFS after encryption.

---

## 2. Creating Peer-to-Peer Network

The blockchain network works using socket programming.

Features include:

* Dynamic node discovery
* Node synchronization
* Permission-based access
* Consensus support
* Network broadcasting

Users join by clicking:

```text
Connect to Blockchain
```

The connected node list updates automatically.

---

## 3. File Key Mechanism

A **File Key** acts as a shared secret between sender and receiver.

Functions:

* Encrypt file during upload
* Decrypt file during download
* Prevent unauthorized access

Supported file formats:

```text
.pdf
.png
.jpeg
.txt
```

Maximum file size:

```text
16 MB
```

---

# IPFS Integration

Blockchain stores only metadata while IPFS stores actual files.

Benefits:

* Lightweight blockchain
* Improved scalability
* Decentralized storage
* Efficient retrieval
* Better accessibility

Workflow:

```text
File Upload
   ↓
AES Encryption
   ↓
Upload to IPFS
   ↓
Generate Hash
   ↓
Store Hash on Blockchain
```

---

# Cryptographic Security

## SHA-256 Hashing

Used for:

* Block hashing
* File hash generation
* Blockchain integrity

Advantages:

* One-way function
* Deterministic output
* Collision resistant
* Fast computation
* Avalanche effect

---

## AES Encryption

AES provides symmetric encryption.

Benefits:

* Shared secret encryption
* Secure file storage
* Protection against unauthorized access

Without AES:

```text
Users could directly access files from IPFS hashes
```

With AES:

```text
Only users with file keys can decrypt files
```

---

# Working Process

## Upload Flow

```text
Sender Uploads File
        ↓
Enter File Key
        ↓
AES Encryption
        ↓
Upload to IPFS
        ↓
Generate Hash
        ↓
Store Hash in Blockchain
```

## Download Flow

```text
Receiver Inputs Hash
        ↓
Enter Correct File Key
        ↓
Retrieve File from IPFS
        ↓
Decrypt using AES
        ↓
Download Original File
```

---

# Experimental Results

Testing was performed using:

* Node A
* Node B

Both nodes:

* Connected to blockchain
* Shared encrypted files
* Downloaded files successfully
* Updated blockchain simultaneously

### Test Scenario

### Test 1

Node A:

```text
Upload File X
Key = P
```

Node B:

```text
Download File X
Using Key = P
```

### Test 2

Node B:

```text
Upload File Y
Key = Q
```

Node A:

```text
Download File Y
Using Key = Q
```

Result:

```text
Blockchain updated successfully on both nodes
```

---

# Advantages

* Decentralized architecture
* Secure storage
* Tamper resistant
* Encrypted sharing
* Lightweight blockchain
* Scalable storage

---

# Future Improvements

* Larger file support
* Mobile compatibility
* Better UI/UX
* Smart contract integration
* Multi-user permissions
* Cloud deployment

---

# Author

## Daksh Bhasin

GitHub:

https://github.com/dakshiitd

---

# License

This project is available for educational and research purposes.

---

If you found this project useful, consider giving it a ⭐

Thank You 😊
