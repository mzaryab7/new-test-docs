# Adding Network to the Wallet

To interact with WireFluid using an EVM wallet such as **MetaMask**, the network must be added manually.

**Steps to Add WireFluid to MetaMask**

1. Open MetaMask and click the **network selector** at the top
2. Select **Add network** → **Add a network manually**
3. Enter the following details:

| Network Name       | WireFluid Testnet            |
| ------------------ | ---------------------------- |
| New RPC URL        | `https://evm.wirefluid.com`  |
| Chain ID           | `92533`                      |
| Currency Symbol    | WIRE                         |
| Block Explorer URL | `https://wirefluidscan.com/` |

4. Click **Save**

Once added, MetaMask will connect directly to the WireFluid network, enabling users to:

* Send and receive WIRE
* Interact with smart contracts
* Use dApps deployed on WireFluid

**Notes**

* Transactions on WireFluid finalize in \~2 seconds due to CometBFT instant finality
* Gas fees are paid in **WIRE** and are typically sub-penny
* Existing Ethereum accounts work seamlessly without reconfiguration
