# How to Use a Bridge

## How to Use a Bridge

Each Presto L2 comes with pre-built in Bridge to the rootchain (L1), protected by zk proofs.

## **What is a blockchain bridge?**

A blockchain bridge is a technology that enables the transfer of digital assets or data between different blockchain networks. It acts as a connection or link between two or more blockchains, allowing them to communicate and interact with each other.

When using a bridge in the context of ZK-rollups, such as Presto layer 2, the bridge serves as a connection between the layer 2 (L2) ZK-rollup and the root chain or layer 1 (L1) blockchain.

The main purpose of a blockchain bridge is to facilitate interoperability and enable the seamless transfer of assets or information across different blockchain platforms. It helps overcome the limitations of isolated blockchains and opens up opportunities for cross-chain transactions and collaborations.

With Presto Platform users can deploy their own zkEVM Rollup on either the Ethereum network or the Gnosis Chain. This rollup will form the basis for creating bridges and achieving scalability.

Blockchain bridges typically consist of a set of smart contracts or protocols that establish trust and enable the secure transfer of assets between blockchains. These bridges ensure that the transferred assets maintain their integrity and security throughout the process.

By using a blockchain bridge, users can leverage the unique features and capabilities of multiple blockchain networks. For example, transfer tokens from one blockchain to another, access decentralized applications (DApps) across different chains, or take advantage of specific functionalities provided by each blockchain.

Blockchain bridges play a crucial role in the development of decentralized finance (DeFi) applications, as they enable the movement of assets between different blockchain-based financial protocols. They also facilitate cross-chain collaborations in various industries, such as supply chain management, gaming, and healthcare.

In summary, a blockchain bridge acts as a vital infrastructure component that fosters interoperability and connectivity among different blockchain networks. It enables the exchange of assets, data, and functionalities, expanding the possibilities and potential of blockchain technology.

## Bridge Functionality in Presto

Blockchain rollups consolidate multiple transactions, processing these transactions off-chain and only forwarding the resultant data to the root chain that can enhance the network's transaction throughput and reduce the cost.It reduces the on-chain transaction load and improves scalability by bundling multiple transactions into a single proof.

ZkRollups facilitate scalability of chains by relocating computation from L1 to L2.

In Presto we will provide the following options:

zkEVM Validium (Proofs on L1): recommended for testing and simple games

zkEVM Rollups (Proofs and DA (data availability) on L1): recommended for projects requiring higher security.

Presto offers easy access to blockchain bridges by facilitating the setting of ZK-rollup. This solution enables quick and effortless deployment of a ZK-EVM rollup, a powerful scaling solution, on either the Ethereum network or the Gnosis Chain. Where you can within minutes get started with:

Deploying private ZK-rollups

Access to block explorers, KYC, indexers & more

L2s & L3, rollups & validiums

For the setup, here’s a documentation guide on [‘How to Create a Rollup’](how-to-create-a-rollup.md). Each Presto L2 comes with a pre-built bridge to the rootchain (L1), which is protected by ZK-proofs.

With Presto, you don't need to manually submit the generated proofs-of-validity or directly interact with the bridge contract on the L1 blockchain. Presto automates this process for you. It handles the submission of proofs-of-validity to the bridge contract and verifies them internally. Once verified, Presto executes the corresponding transactions on the L1 blockchain seamlessly and securely.

Presto automatically deploys a bridge contract on the main blockchain (layer 1) to serve as an interface between the ZK-rollup and the main chain. The bridge contract defines the rules and protocols for transferring assets or executing transactions between the two chains. As seen in [this bridge contract example on Seopolia Blockscout](https://eth-sepolia.blockscout.com/address/0x8DA0B6b941B8c70827081Be613fC8b0eA1f0a9F6?tab=txs).

General process for how a Presto ZK-rollup can connect to a blockchain bridge:

1. Setup Presto Bridge: The ZK-rollup contract sets up a bridge contract on the main blockchain. This bridge contract is responsible for receiving and validating proofs from the ZK rollup.
2. Off-chain Transaction Processing: When users initiate transactions on the ZK-rollup, the transactions are aggregated and bundled into batches off-chain.
3. Generating Proofs-of-Validity: Once the transactions are bundled, the ZK-rollup generates a cryptographic proof-of-validity. This proof demonstrates that all the transactions within the rollup are valid according to the ZK-rollup’s rules and protocols.
4. Proof Submission: The ZK-rollup submits the proof-of-validity to the bridge contract on the main blockchain through the blockchain bridge.
5. Proof Verification and Execution: The bridge contract, facilitated by Presto, verifies the proof-of-validity and ensures that all the transactions within the ZK-rollup are valid and comply with the main blockchain's rules. If the proof is valid, the bridge contract executes the transactions on the main blockchain.
6. User-Friendly Interface: Presto offers a user-friendly interface that simplifies the interaction with the blockchain bridge. Users can easily initiate transactions, monitor their progress, and track their transaction history within the Presto platform. The intuitive design and comprehensive features make it accessible even for non-technical users.

With Presto, the ZK-rollup achieves seamless connectivity to the main blockchain through the blockchain bridge. The bridge, enabled by Presto, acts as an intermediary facilitating secure communication and data transfer between the ZK-rollup and the main blockchain. Users can explore and analyze the executed transactions and associated data using Presto's built-in default explorer Blockscout, a powerful tool for blockchain data analysis. For custom solutions, any other block explorer can be integrated.

### How to Use A Presto Bridge (Bridging L2 to L1)

After you’ve connected to the public rollup sn2-Stavanger (root chain Ethereum Sepolia) Testnet with your MetaMask wallet, the next step is to send ETH via Faucet. When transferring from L2 to L1, the bridge on L1 can’t mint tokens. Therefore, the bridge smart contract must be funded before bridging can occur. For example, you can’t bridge from L2 to L1 until you send test Sepolia tokens to this bridge smart contract via a faucet. After the bridge smart contract has been funded, you can bridge a maximum amount equal to the amount funded from L2 to L1. On the other hand, when transferring from L1 to L2, you don’t need to fund the bridge smart contract.

1.Go to Bridge Section in presto.gateway.fm:

<figure><img src="../../.gitbook/assets/Bridge_1.png" alt=""><figcaption></figcaption></figure>

2..Go to a Bridge URL and Add your rollup/validium to your wallet

<figure><img src="../../.gitbook/assets/Bridge2.jpeg" alt=""><figcaption></figcaption></figure>

3. Go to ETH Faucet and type your address to receive 1 ETH.

<figure><img src="../../.gitbook/assets/bridge_3.jpeg" alt=""><figcaption></figcaption></figure>

4. Bridge 1ETH to Ethereum  Sepolia

<figure><img src="../../.gitbook/assets/bridge_4.jpeg" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/bridge_5.jpeg" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/bridge_6.jpeg" alt=""><figcaption></figcaption></figure>

5. In your Presto Bridge you will see the funds and from here you can bridge your ETH. Choose from where and the amount. Click ‘bridge’ and then confirm in your MetaMask wallet. Within Presto L2, you can execute off-chain transactions. These transactions are processed and verified using ZK-proofs, which ensure the validity and integrity of the transaction history. Once the transactions are processed, cryptographic proofs-of-validity are generated.
6. The activity will be processed and after that you can see the Bridge details.

<figure><img src="../../.gitbook/assets/bridge_7.jpeg" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/bridge_8.jpeg" alt=""><figcaption></figcaption></figure>

7. The details are also available on the blockchain explorer. Once the proofs are validated, the transactions are executed on the L1 blockchain, providing trust and security. This can be observed by examining the transaction history and state changes on the L1 blockchain via block explorers or any other interface provided by the blockchain network.

<figure><img src="../../.gitbook/assets/bridge_9.jpeg" alt=""><figcaption></figcaption></figure>

By using the bridge on Presto, you get the benefits of increased scalability, reduced transaction fees, and improved privacy, as most of the transaction processing occurs off-chain within the ZK-rollup.

### How to Use A Presto Bridge (Bridging L1 to L2)

This guide will reverse the process from above by bridging from L1 to L2. The Presto bridge enables seamless connectivity and secure transfer of assets between L1 and L2 blockchain.

1. Use Sepolia to send ETH to your MetaMask. Before you can bridge from L1 to L2, ensure that you have received ETH in your MetaMask wallet, which is connected to the Presto Bridge.

<figure><img src="../../.gitbook/assets/br1.jpeg" alt=""><figcaption></figcaption></figure>

Upon receiving the ETH in your MetaMask wallet, since it’s connected to the Presto Bridge it will automatically proceed the bridging.

2. Select the 'from' and 'to' options, along with the desired amount to be bridged. Click 'bridge' to initiate the process.

<figure><img src="../../.gitbook/assets/br2.jpeg" alt=""><figcaption></figcaption></figure>

3. This prompt will ask you to write “I Understand” before continuing. In your MetaMask wallet, confirm the bridge transaction by following the prompted instructions.

<figure><img src="../../.gitbook/assets/br3.jpeg" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/br4.jpeg" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/br5.jpeg" alt=""><figcaption></figcaption></figure>

4. Once the bridge transaction is completed, you can view the details of the bridged transaction on the built-in blockchain explorer.

<figure><img src="../../.gitbook/assets/br6.jpeg" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/br7.jpeg" alt=""><figcaption></figcaption></figure>

With Presto, you can enjoy increased scalability, reduced transaction fees, and improved privacy. The majority of transaction processing occurs off-chain within the ZK-rollup, providing a secure and efficient user experience.

#### Summary:

How to use a bridge in ZK-rollups:

In Presto L2, off-chain transactions can be executed. These transactions are processed and verified using ZK-proofs, ensuring the validity and integrity of the transaction history. Besides proofs, for rollups, data availability (DA) is also sent to L1. This means that not only cryptographic proofs-of-validity are generated, but also the necessary data is made available on the Layer 1 blockchain.

Presto L2 is equipped with a pre-built bridge that connects the ZK-rollup to the root chain/ L1 blockchain. The bridge is responsible for receiving and validating the generated proofs-of-validity before executing the transactions on the L1 blockchain.

Once the proofs are validated, the transactions are executed on the L1 blockchain, providing trust and security. This can be observed by examining the transaction history and state changes on the L1 blockchain via block explorers. Presto Layer 2 (L2) solution includes a built-in block explorer, providing users with a robust tool to effortlessly explore and analyze blockchain data.

By using the bridge on Presto, you get the benefits of increased scalability, reduced transaction fees, and improved privacy, as most of the transaction processing occurs off-chain within the ZK-rollup.
