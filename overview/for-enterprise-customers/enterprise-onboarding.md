# Enterprise Onboarding 33fbd69df36d42afbfa167c745029e7b

## Enterprise Onboarding

see also [How to Become an Enterprise Customer?](https://www.notion.so/How-to-Become-an-Enterprise-Customer-399550f40c1f4dfc9f8e11263f7c246f?pvs=21) and [Enterprise vs Paid — what is the difference?](https://www.notion.so/Enterprise-vs-Paid-what-is-the-difference-eea20637f5334261a600f2fcbe8c778f?pvs=21)

## 1. Testing on a private validium (optimistic mode)

Client creates their own validium in Presto (https://presto.gateway.fm) with the settings they want.

Client sends us their email, we can prolong the trial period to what is needed.

We also exclude this client from the inactivity removal of the rollup.

Information about RPCs, Block explorer, faucet, etc — everything is available in the rollup details.

No real zk prover here, the network works in the optimistic mode.

\*This step could be **free** for the client, but time-limited. \~2-4 tps (\*see [What are the conditions of the trial](https://www.notion.so/What-are-the-conditions-of-the-trial-01b77be4a9d447d5886a8fef4835c948?pvs=21))

## 2. (optional) Testing on Stavanger Public Testnet

If needed, tests and development could happen on the Stavanger Public Testnet, but if a client really needs a zk prover, Stavanger is a good option.

## 3. (Optional) Customized Testnet

If any of a special customizations are needed for the client:

* more powerful servers
* specific L1/rootchain
* _rollup mode (instead of validium)_
* _real zk-prover_
* custom fork of CDK/zkEVM
* custom gas token
* special software or unique partners alongside rollup (indexers, their own kyc, bridges etc)
* other customizations

Then Gateway team can provision on demand a special customized testnet, at extra cost. This testnet’s liveness depends on the agreement.

This customized testnet is then added to the client account to Presto. 10+ tps

## 4. Mainnet Provisioning

After developing and testing on either a private validium or Stavanger Public Testnet — client requests the provisioning of the right configuration of the rollup.

Gateway team provisions it manually, and adds it to the client account to Presto.

## Technical Support

A shared TG group or a Slack channel is created with the client to help them onboard and use Rollups by Presto.
