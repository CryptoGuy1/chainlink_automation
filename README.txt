# ⛓️ Chainlink Automation Showcase – Time-Based, Custom Logic & Log-Triggered Upkeeps

This repository contains a collection of smart contracts deployed on the **Sepolia** and **Chainlink (LINK)** test networks. It demonstrates various types of Chainlink Automation (formerly Keepers) use cases — including time-based upkeeps, custom logic triggers, and log-triggered executions.

> These contracts serve as modular examples for developers looking to integrate reliable, decentralized automation into their Web3 applications.

---

## 📌 Overview

Chainlink Automation allows smart contracts to be automatically executed based on conditions defined by the contract creator. In this repo, four key automation patterns are demonstrated:

| Contract         | Description                                                                 |
|------------------|-----------------------------------------------------------------------------|
| `TimeBased.sol`   | Simplest contract; increments a counter — can be triggered externally.      |
| `CustomLogic.sol` | Implements on-chain time-interval logic and self-managing upkeep behavior.  |
| `EventEmitter.sol`| Emits logs that simulate event-based triggers for external automation.      |
| `LogTrigger.sol`  | Listens for specific logs and reacts accordingly using custom log decoding. |

---

## 🧠 Use Case Scenarios

| Contract         | Automation Type     | Real-World Application Example                    |
|------------------|---------------------|---------------------------------------------------|
| `TimeBased.sol`   | External time-based | Scheduled tasks like hourly payouts or rebalances |
| `CustomLogic.sol` | Internal logic-based| Polling-based logic (e.g., price feeds, timers)   |
| `EventEmitter.sol`| Log producer        | User action signals, alerts, on-chain events      |
| `LogTrigger.sol`  | Log consumer        | Reactive upkeeps based on event emissions         |

---

## 🧪 Deployed Networks

These contracts have been deployed and tested on:

- ✅ **Sepolia** Testnet  
- ✅ **Chainlink Automation (LINK) Test Network**  
  - via [Chainlink Automation App](https://automation.chain.link/)

---
🧪 How to Register Upkeeps
Go to Chainlink Automation App

Connect your wallet (on Sepolia)

Register a new upkeep:

For TimeBased or CustomLogic: use checkUpkeep & performUpkeep

For LogTrigger: set a log trigger based on events from EventEmitter

Fund the upkeep with test LINK (from faucet)

