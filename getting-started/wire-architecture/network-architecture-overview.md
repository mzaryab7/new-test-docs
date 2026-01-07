# Network Architecture Overview

WireFluid is implemented as a **standalone Cosmos SDK app-chain** with an embedded **Cosmos EVM module**.

#### High-Level Stack

```
                                ┌─────────────────────────────┐
                                │ Applications                │
                                │ DeFi • Payments • NFTs      │
                                ├─────────────────────────────┤
                                │ WireFluid (EVM Layer)       │
                                │ Solidity • JSON-RPC         │
                                ├─────────────────────────────┤
                                │ WireCosmos                  │
                                │ Bank • Staking • Gov • IBC  │
                                ├─────────────────────────────┤
                                │ CometBFT                    │
                                │ Instant Finality Consensus  │
                                └─────────────────────────────┘
```

### Consensus & Security

* **Consensus Engine:** CometBFT
* **Consensus Model:** Delegated Proof-of-Stake (DPoS)
* **Finality:** Instant finality (\~2 seconds per block)
* **Validator Selection:** Stake-weighted

This design provides Byzantine Fault Tolerance (BFT) with fast confirmation and strong economic security.
