# How To Use Presto with ethers.js

To use Presto with ethers.js using a custom RPC endpoint, follow these steps:

1. Install the ethers.js library by running `npm install ethers` in your project directory.
2. Create your rollup ([How to Create a Rollup](https://www.notion.so/How-to-Create-a-Rollup-e3df7836e3944c61a97e516134d43a90?pvs=21)), open it and get the RPC url ([What Is RPC](https://www.notion.so/What-Is-RPC-094669c329814c6a92d7acbae84d5d3c?pvs=21))
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
