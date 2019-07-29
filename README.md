# validator-workshop

Welcome to the accompanying assets to the Validator Workshop. In this repository you'll find written instructions and the necessary `chainspec.json` for connecting to the test network and run a validator.

## About the testnet

This is a public testnet set up by Web3 Foundation for the purpose of allowing people to try being validators. It is more up-to-date with the latest code than the Alexander testnet and will be nearly identical to the experience of validating on a live chain. We will not keep this testnet running forever so don't be surprised when it eventually gets turned off.

## How to run

Docker is required. If you do not have Docker installed please consult the [Docker documentation](https://docs.docker.com/install/) or make some searches containing the keywords "<your operating system> docker install" and there is likely a detailed guide on installing Docker to be found.
  
We will be using the latest Polkadot image from Parity. You can pull this image from the Docker Hub like so:
```
$ docker pull parity/polkadot
```

If this command failed, your installation of Docker did not go right, return to the search engine and solve your problem. If you pull the image correctly, then the rest of this tutorial should work for you.

Next you need to get the `chainspec.json` provided in this repo.

## Using the Polkadot UI

Navigate to the [Polkadot UI](https://polkadot.js.org/apps/#/explorer).

Change your settings in the `Settings` tab to use a custom endpoint and input `wss://validator-testnet-0.w3f.tech`.
