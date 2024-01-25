# How to use Presto with ethers.py

1.  Create your rollup ([How to Create a Rollup](../main-functionality/how-to-create-a-rollup.md)), open it and get the RPC url ([What Is RPC](what-is-rpc.md))\


    <figure><img src="../../.gitbook/assets/web3_js.png" alt=""><figcaption></figcaption></figure>
2. Set up a custom RPC endpoint:

To use Presto with [ethers.py](http://ethers.py/), you can set up a custom RPC endpoint using the following code:

```python
from ethers import JsonRpcProvider

url = "<L2 RPC URL>"

gatewayHttpProvider = JsonRpcProvider(url)

```
