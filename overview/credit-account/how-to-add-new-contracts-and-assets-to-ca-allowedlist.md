---
description: Guidance for adding new assets and contracts to the AllowedList.
---

# How to add new Contracts & Assets to CA AllowedList

{% hint style="info" %}
Composability is at the heart of Gearbox Protocol's ethos as well as its modular architecture. It's imperative to grow the Allowed List Policy to allow traders & farmers to create composable positions across DeFi and other sectors. While the protocol is growing, there are some technical boundaries in place with regard to things like oracles when it comes to assets as well as contracts - to understand those better, please see some wishlist for Gearbox DAO below. If it checks out, go ahead and ask DAO to add it!&#x20;

* Discord chat to ask tech questions is [here](https://discord.gg/JZgvmaenwn).

If you would like to have an adapter and believe you don't have enough resources to build it yourself, please just ping on Discord & let's collab together on a grant to have an external or internal developer help with such a task! Cooperation is welcome :-)
{% endhint %}

This article can give you an insight on how you can potentially access a collateral / protocol:

{% embed url="https://medium.com/gearbox-protocol/risk-committee-daos-framework-for-accessing-assets-contracts-3d4deea83537" %}

Dev docs will help you fully understand the architecture:

{% embed url="https://dev.gearbox.fi/" %}

GitHub repositories can show you examples of live integrations:

{% embed url="https://github.com/Gearbox-protocol/integrations-v3" %}

## Add new Contracts / Protocols

#### Technical Requirements

* (preferably) The Protocol should have at least two external audit reports.
* (preferably) Adapter for the Protocol should have at least one external audit report.
* (preferably) The Protocol should be at least 2 months from the launch and 2 months without security incidents.
* (preferably) The protocol should be non-custodial.
* Integrations should be made using ERC-20 token in the middle. It could be LP token of Protocol (or in the case of absence LP tokens, should be created separate ERC-20 token that represents user’s position in Protocol). Later on, more standards can be added to expand. Please propose.
* It’s good if methods how LP token can be priced (via using internal/external oracle / using smart contract interface like pricePerShare for Yearn Vaults) are described in the application.
* It is also necessary to show why the price cannot be manipulated and/or describe how to mitigate such risks. It is good to describe how the withdrawal of funds from the protocol works: is it instantaneous, whether funds are locked there, for what period.

#### Step by step process

1. Create a discussion on Discord Forum.

* (preferably) include links to the code of the Adapter to integrate with external protocol. If there are none, the discussion can be continued, but any other actions can be made after someone (community, post author etc) provide link to Adapter implementation.
* (preferably) include links to external audit of Adapters. If there are none, the discussion can be continued, but the vote can be submitted only after receiving the audit report.

2\. After initial discussions it is possible to go through the [standard governance process](../../governance/setup/).

{% hint style="success" %}
Prior to the forum posts, feel free to ping on [Discord](https://discord.gg/JssNVvxscK) to ask for help!
{% endhint %}

## Add new Assets / Tokens&#x20;

#### Technical Requirements

* It should be an ERC20 token.&#x20;
* (required) Must have a [chainlink price feed oracle](https://docs.chain.link/docs/ethereum-addresses/) for the token. As you might have guessed, this is the oracle system Gearbox Protocol uses on Ethereum and in its current version.
* (preferably) not possible to pause tokens fully or freeze individually.
* (preferably) fee-on-transfer and rebase tokens to be avoided.
* (preferably) the token must be liquid and have big depth on the secondary markets, specifically DEXes. This is one of the protections against the domino effect.

Risk requirements:&#x20;

* Volatility should be low enough to get leverage. Current approach is the following:&#x20;

1. Check 5 Min max price drop for the last 12 months. Health value is less than 20%.&#x20;
2. See parameters of this token on notable DeFi money markets / lending services and whether liquidators manage to eliminate positions in this token with such parameters (if applicable).&#x20;

* Liquidity should be enough to be able to liquidate positions.
* Optimal distribution of tokens (number of holders, distribution of tokens, unlocking schedule).

#### Step by step process

1. Create a discussion on Discord Forum inside "discussions" tab. Preferably, the first post should include data of token volatility for the last 1 year and of token liquidity.&#x20;
2. After initial discussions it is possible to go through the [standard governance process](../../governance/setup/).&#x20;

{% hint style="success" %}
Prior to the forum posts, feel free to ping on [Discord](https://discord.gg/JssNVvxscK) to ask for help!
{% endhint %}
