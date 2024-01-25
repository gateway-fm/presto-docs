# How To Use Presto with ethers.js

To use Presto with ethers.js using a custom RPC endpoint, follow these steps:

1. Install the ethers.js library by running `npm install ethers` in your project directory.
2.  Create your rollup ([How to Create a Rollup](../main-functionality/how-to-create-a-rollup.md)), open it and get the RPC url ([What Is RPC](what-is-rpc.md))\


    <figure><img src="../../.gitbook/assets/web3_js.png" alt=""><figcaption></figcaption></figure>
3. Set up a provider to connect to your Presto L2 network using your custom RPC endpoint
4. Make sure to replace `YOUR_CUSTOM_RPC_ENDPOINT` with the URL of your custom RPC endpoint.

```jsx
const { ethers } = require('ethers');

const provider = new ethers.providers.JsonRpcProvider('YOUR_CUSTOM_RPC_ENDPOINT');

async function getBlockByNumber(blockNumber) {
  try {
    const block = await provider.getBlock(blockNumber);
    console.log(block);
  } catch (error) {
    console.log(error);
  }
}

getBlockByNumber(12345);

```
