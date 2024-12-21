# cdp-docs

I gave setting up the SDK and getting started with creating/funding a wallet a try (Python only). I was able to successfully complete the Quickstart, but I created this repository with an example of how I would approach a document like this.

- [`getting-started.md`](getting-started.md): I broke this out into a smaller guide that doesn't include wallet setup. It can be treated as a prerequisite in additional guides. This is a modification of [Getting Started](https://docs.cdp.coinbase.com/get-started/docs/use-sdks).
- [`backend-create-wallet`](backend-create-wallet.md): I went through this tutorial on my own in order to figure out how to better organize it. This is a modification of [Quickstart (for MPC wallets)](https://docs.cdp.coinbase.com/mpc-wallet/docs/quickstart). 

Below are some quick notes on improvements.
## Consolidate repeated information

There are steps a part of the backend SDK quickstart that are also included in the Getting Started page. This isn't necessary IMO, better to split them apart and keep them separate.

Likewise, the Getting Started guide repeats steps from the Quickstart, repeating the same docs in two separate places.

I think it makes more sense for Getting Started to be more lightweight, bare minimum and point to users to additional guides, with Getting Started as a prerequisite.
## Keep an example repo

I would store all code examples in an example repo if they aren't already. You can keep them as separate projects or scripts, but at the end of each tutorial you can link to it in case others want to view the project in full. 

It's also easier to keep the project/docs up-to-date this way (could even automate it by injecting the examples from the repo, to keep things in sync if an example gets updated).
## Clarify step-by-step instructions

The Quickstart covered everything I needed to know, but it wasn't clear at first that these are step by step instructions. I modified the headers into logical chunks to help with that.

## Bring attention to persisting a wallet

If suggesting a best practice or recommendation, I would include this as a part of the Quickstart guide directly. I think this could help increase developer trust in the product, especially around potentially dangerous actions that might cause you to lose access to your wallet.

Also, the link in the Getting Started guide that points me to these directions has a broken anchor (section no longer exists). I think this set of instructions on wallet persistence could also use some work. 

## Add (or link to) more contextual information

The guides could add more contextual information on various topics. I like to assume a developer may have never used technology like this before, it increases ease of adoption in my opinion. 

If assuming the audience is more advanced, you could add this to the prerequisites as an assumption. Otherwise, you could create some brief blurbs with contextual overviews, or just link out to existing docs. 

Some might argue this information does not belong in a Quickstart, though.





