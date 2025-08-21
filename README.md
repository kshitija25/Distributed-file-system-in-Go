# Distributed File System in Go

A lightweight **peer-to-peer distributed file system** written in Go.  
This project is designed as a learning exercise in distributed systems, networking, and storage primitives.

## ✨ Features
- Run multiple nodes and connect them via TCP
- Store and retrieve files through a distributed interface
- Basic peer-to-peer messaging (handshake, request, response)
- Simple local storage abstraction for managing files
- Includes unit tests for core storage and transport modules

## 🚀 Getting Started

### Prerequisites
- Go 1.22+ → https://go.dev/dl/

### Build
    go build -o dfsnode .

### Run a node
    ./dfsnode

By default, nodes listen on ports **3000**, **5000**, and **7000** for peer communication.

## 🧪 Example Usage
1. Start multiple nodes in different terminals:

       ./dfsnode

2. The nodes will attempt to connect with each other over TCP.  
3. Files written to one node are propagated to peers.

