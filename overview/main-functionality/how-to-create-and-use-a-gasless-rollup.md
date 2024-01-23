# How To Create & Use a Gasless Rollup

## What is a Gasless Rollup?

In a gasless rollup, users can opt-out to set up gas price to 0. That way they don’t have to even have tokens to be able to transact on the gasless blockchain.

Gas fees are covered by the user then.

Downsides of this approach is opening up to spamming the network.

## How to Deploy a gasless rollup

1. Deploying a gasless rollup follows the same process as How to [Create a Rollup](how-to-create-a-rollup.md), except you select “Gasless/No fees” as an option.
2. When sending transactions to the network, set `gasPrice` to `0`.
