# Introduction
This repository implements simple blockchain using [TypeScript](https://www.typescriptlang.org). It is a rewrite of the original one created in Python from this [article](https://hackernoon.com/learn-blockchains-by-building-one-117428612f46).

# Usage
Run `npm start -- -port <port-number>` to start the blockchain node.

# Develop
Run `npm run tsc:watch` to start TypeScript compiler and run `npm run watch` to start node in watch mode.

# Proof of Work algorithm
Blockchain implements basic Proof of Work algorithm. Miners need to find a number that, when hashed with the previous block’s solution (proof), creates a hash with 4 leading 0s ('0000').  
Blockchain class methods *proofOfWork* and *validProof* implements Proof of Work algorithm.

# Consensus algorithm
Consensus algorithm ensures that all nodes in decentralized network reflect the same blockchain. Rule of Consensus algorithm is that the longest valid chain is authoritative. It is achieved by sending the whole chain to each of the nodes.

