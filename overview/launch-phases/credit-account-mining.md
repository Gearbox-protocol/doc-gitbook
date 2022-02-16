---
description: Help deploy a piece of the protocol and get GEAR!
---

# Credit Account Mining

{% embed url="https://medium.com/gearbox-protocol/credit-account-mining-guide-fueling-up-for-the-launch-abc17fbddbad" %}
ALL YOU NEED TO KNOW
{% endembed %}

{% embed url="https://youtu.be/2DZafHnECXs" %}

{% hint style="info" %}
One of the coolest Gearbox DAO launch parts is here!&#x20;

**TLDR: deploy a piece of the protocol by paying gas fees => get GEAR tokens in return.**

Each one of the eligible addresses can deploy 1 Credit Account only, for fixed 100,000 GEAR in return. 5% for 5,000 accounts. Learn more below and in [GEAR token page](broken-reference).
{% endhint %}

{% embed url="https://etherscan.io/address/0x7B1AAF21AC0D420666B5966338FF9aEe763C29DF#code" %}
[https://etherscan.io/address/0x7B1AAF21AC0D420666B5966338FF9aEe763C29DF#code](https://etherscan.io/address/0x7B1AAF21AC0D420666B5966338FF9aEe763C29DF#code) - AccountMining
{% endembed %}

### How the ceremony was designed

The goal of Credit Account Mining ceremony is to restock the factory of [Credit Accounts](../credit-account/) that leverage users can “rent” from Gearbox Protocol later on. This way, leverage users won’t need to deploy expensive smart contracts every time, but instead just rent and give it back to the protocol after closing or being liquidated - this makes the protocol gas efficient! See more in the [tech paper](../whitepaper.md).

_Looking at the unique DeFi users on mainnet, the numbers are still in the low 4 digits (below 10K per protocol, at best). We don’t expect Gearbox Protocol to be an exception to this just yet, because the protocol is not even live yet! But we also want to make sure the protocol has enough accounts for the first few months. After all, some accounts don’t get closed, some people might open a few at a time, and so on. Therefore, a number of 5,000 accounts to start with - seemed logical. If more are to be needed later on, another ceremony in an auction model could be held, for example, or just deploying from DAO Treasury funds._

Then, how does one choose who is eligible for it? And now we are getting back to the objective of the CA Mining ceremony: we already have the [early testers and early community list](early-drop.md), we have some [early developers](broken-reference), and some early contributors… So for this ceremony, we decided to include governance participants of other protocols. This achieves the following: (i) choosing users who are familiar with governance and have voted before, so they potentially could be good for Gearbox DAO; (ii) visibility from other community because they are being given a cool chance to take part in the very first days of another DeFi protocol for potential integrations later on ; (iii) slightly works as an anti-sybil mechanism to make sure 1 group doesn’t take the entire supply into their hands.

### Some facts about the Credit Account Mining ceremony

With 5,000 max Credit Accounts possible at this stage, not everyone will be able to participate in this exact distribution ceremony - which is okay, there will be other opportunities. However, the list needs to stay large enough to account for the fact that many of said wallets will either be inactive, or they won’t know of this ceremony, and so on. The gap could be like 5x of the total amount possible, to make sure that if there is demand - it should be met with the said wallets.

* There is an approximately 48 hour window for this ceremony, after which the DAO votes shall begin. However, if not all 5,000 Credit Accounts are mined within the 48 hour period - they will remain there to be mined by the same wallet list (nothing will change with regard to that). So the window is not anyhow enforced, it's simply there to start DAO votes asap. If there is not enough for such a ceremony at the start, eligible wallets can decide to mine remaining later.
* Because of pre-baked extra token approvals in the Credit Account Smart Contracts that will make the lives of protocol users easier later on, it costs approximately 2.5M gas to deploy one such SC. That is approximately 0.25ETH in deployment costs at current gas prices of 100. This of course can vary depending on network congestion. The mining is based on FCFS.

{% hint style="warning" %}
With the current Ethereum block limit of 30M gas, there can be at maximum 12 Credit Accounts in a block. However, as every block has other important launches, liquidations, etc. - it's likely the number will be lower. This could potentially clog Ethereum for a few hours and make gas costs go up. Let's say 7 accounts per block \* 15 second block = 35 accounts per minute => 2,100 accounts per hour. Technically, can be done in 3 hours.

We apologize for such a design of the ceremony, but it was actually a calculated risk: if done differently, users would have to deploy and then throw away their Credit Accounts every single time, causing much more wasteful gas usage. With the model in place though, there is this one-time event which clogs the network, but at least after that users would be able to just rent Credit Accounts and thus make the network a bit less clogged.
{% endhint %}

The list of eligible addresses and the conversation was taking place here:

{% embed url="https://gov.gearbox.fi/t/credit-account-mining-snapshot-list/18" %}

### Who is on the list?

1. Lobsterdao NFT holders as an appreciation to the early community who have helped with ideas and support. We did not see people transferring NFTs to multiple wallets (in order to sybil) so there was no extra action taken yet to sort this out. Please cross-check. _No 10+txs requirement._
2. Snapshot governance of protocols were taken with 10+ transactions per wallet. We thought this would be a good way to filter out _possible_ bot accounts, but this might be a wrong approach. Another way to go about it would be doing minimum balances. Or doing some wallet cross-checks… Please suggest, run tests, and comment.

* 1inch.eth
* Alchemixstakers.eth
* Bancornetwork.eth
* Convex
* Cream-finance.eth
* Dydxgov.eth
* Fei.eth
* Gitcoindao.eth
* Index-coop.eth
* Lido-snapshot.eth
* MIM
* Olympusdao.eth
* Powerpool
* Rari Capital
* Ribbon.eth
* Snxambassador.eth
* Snxgov.eth
* Spartancouncil.eth
* Sushigov.eth
* Tokemak
* Yearn.eth
* Ybaby.eth

On-chain governance of:

* ENS delegates
* COMP delegates
* UNI delegates
* veCRV holders
* MakerDAO voters
* Aave voters
* Nexus Mutual voters

And also:

* Element Finance LPs with 10+ transactions per wallet
* GTC claimants with 10+ transactions per wallet

{% hint style="success" %}
You can also find more information here with snapshots and dune queries:
{% endhint %}

{% embed url="https://github.com/Gearbox-protocol/launch-snapshot" %}
