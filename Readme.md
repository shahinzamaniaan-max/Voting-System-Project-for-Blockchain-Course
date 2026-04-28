# 🗳️ Decentralized Voting System (Ethereum Smart Contract)

## 📌 Overview
This project implements a decentralized voting system using Solidity and Ethereum blockchain. The system ensures transparency, immutability, and security in the voting process.

## 🚀 Features
- One vote per address
- Immutable vote storage
- Candidate management (owner-only)
- Real-time result tracking

## 🛠️ Tech Stack
- Solidity
- Remix IDE
- MetaMask
- Ethereum Sepolia Test Network

## ⚙️ Smart Contract Structure

```solidity
struct Candidate {
    string name;
    uint voteCount;
}

mapping(address => bool) public hasVoted;
Candidate[] public candidates;
address public owner;