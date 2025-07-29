# Polymarket User and Temporal Behavior Analysis

## Overview

This project focuses on the analysis of **user behaviors and temporal patterns** on [Polymarket](https://polymarket.com), a blockchain-based prediction market platform. It aims to uncover insights into how users interact with markets over time and how events influence trading dynamics.

## Dataset Description

The core dataset consists of:

- **Market transaction data** from the Polygon blockchain, including:
  - ERC-20 (USDC) token transfers
  - ERC-1155 event logs representing prediction market share trades
  - Market metadata (YES/NO shares, resolution time, market categories)

- **User historical activity**, including:
  - Trading patterns across multiple markets
  - Profit and loss history
  - Participation in specific event-driven markets

Data is collected and parsed directly from on-chain sources to ensure transparency and verifiability.

## Technical Components

To support large-scale and historical data analysis, this project includes:

- **Deployment of a full Polygon archive node**, using:
  - [Erigon](https://github.com/ledgerwatch/erigon) with archive settings for efficient historical queries
  - `eth_getLogs` and other RPC methods for extracting contract-level event data

- **Data extraction tools**:
  - Scripts to parse ERC-20 and ERC-1155 transfer logs
  - User-level aggregation logic for market-wise behavior analytics

## Use Cases

- Understanding trading behavior around major real-world events
- Detecting user strategy patterns (e.g., timing, spread trading)
- Analyzing market efficiency and liquidity dynamics on Polymarket

## Acknowledgments

This project is not affiliated with Polymarket. It uses public blockchain data for academic and analytical purposes only.

---

Feel free to open an issue or submit a pull request for improvements or questions.
