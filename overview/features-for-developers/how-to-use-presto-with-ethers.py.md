# How to use Presto with ethers.py

1. Create your rollup ([How to Create a Rollup](https://www.notion.so/How-to-Create-a-Rollup-e3df7836e3944c61a97e516134d43a90?pvs=21)), open it and get the RPC url ([What Is RPC](https://www.notion.so/What-Is-RPC-094669c329814c6a92d7acbae84d5d3c?pvs=21))
2. Set up a custom RPC endpoint:

To use Presto with [ethers.py](http://ethers.py/), you can set up a custom RPC endpoint using the following code:

```python
from ethers import JsonRpcProvider

url = "<L2 RPC URL>"

gatewayHttpProvider = JsonRpcProvider(url)

```
