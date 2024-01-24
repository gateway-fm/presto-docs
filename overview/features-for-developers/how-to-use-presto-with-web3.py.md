# How to use Presto with web3.py

1. Create your rollup ([How to Create a Rollup](https://www.notion.so/How-to-Create-a-Rollup-e3df7836e3944c61a97e516134d43a90?pvs=21)), open it and get the RPC url ([What Is RPC](https://www.notion.so/What-Is-RPC-094669c329814c6a92d7acbae84d5d3c?pvs=21))

```python
from web3 import Web3

presto = Web3(
    Web3.HTTPProvider(
        "<L2 RPC URL>"
    )
)
```
