# How To Use Presto with viem.sh

To use Presto with [viem.sh](http://viem.sh/) library using a custom RPC endpoint, follow these steps:

1. Install the [viem.sh](http://viem.sh/) library by running `npm install viem.sh` in your project directory.
2.  Create your rollup ([How to Create a Rollup](../main-functionality/how-to-create-a-rollup.md)), open it, and get the RPC URL ([What Is RPC](what-is-rpc.md)).\


    <figure><img src="../../.gitbook/assets/web3_js.png" alt=""><figcaption></figcaption></figure>
3. Set up a provider to connect to your Presto L2 network using your custom RPC endpoint.
4. Make sure to replace `YOUR_CUSTOM_RPC_ENDPOINT` with the URL of your custom RPC endpoint.

```jsx
const { viem } = require('viem.sh');

const provider = new viem.providers.JsonRpcProvider('YOUR_CUSTOM_RPC_ENDPOINT');

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
