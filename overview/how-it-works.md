---
description: High-level technical overview of Gearbox Protocol.
---

# How it works

Gearbox protocol has two sides to it:

* **Passive lenders:** **asset** **lenders** who seek passive yield and prefer lower risks. This can be seen similar to providing liquidity to Compound and getting cTokens back. Lenders' assets are utilized by others, for which they get APY. Any one can be a liquidity provider on Gearbox. [See how](../lending-market/manage-liquidity.md).
* **Borrowers** - **active** **traders, farmers, and even protocols** who wish to increase their position by borrowing liquidity from the protocol at multiples of their collateral. The liquidity they borrow can be 10x of what their notional size is. This is the leverage power! [See how](../traders-and-farmers/strategies/).

## Core Parts of Gearbox Protocol

<figure><img src="../.gitbook/assets/Screenshot 2021-08-07 at 22.53.18.png" alt=""><figcaption></figcaption></figure>

One of the key aspects which actually makes this DeFi primitive possible are [Credit Accounts](credit-account/) (and Credit Managers), which “bind” together lenders and borrowers in this equation. More specifically, a Credit Account is an isolated smart contract (like a leveraged smart contract wallet) that holds user + borrowed funds, has liquidation thresholds, and **has a list of** [**Allowed Tokens and Protocols**](credit-account/#allowed-list-policy) (in order to avoid attack vectors from malicious actors, like borrowing leverage and buying a self-created ERC20 token; or sending an amount to a malicious smart contract).

{% content-ref url="credit-account/" %}
[credit-account](credit-account/)
{% endcontent-ref %}

**Gearbox does not silo the assets within its protocol.**&#x20;

All trades and farming operations happen on third-party protocols: Uniswap, Curve, Yearn, etc. **Your assets never end up in custody of any one person or company**. As such, Gearbox Protocol is not a trading platform / protocol. The protocol does not have its own order books, or control the secondary market liquidity. Therefore, there are no funding rates.

Integrations possibilities are very broad, as Gearbox is built with composability at its core:

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

The positions which traders and farmers take should be liquidated by third-party [liquidators](liquidations/) before the assets of liquidity providers would start being exposed to the downside. As such, the protocol returns the liquidity providers’ assets to the pools if all functions correctly and liquidators do their job. This is how Gearbox is able to provide composable leverage.&#x20;

The liquidations are based on the **health factor and the threshold weighted value**:

{% content-ref url="liquidations/" %}
[liquidations](liquidations/)
{% endcontent-ref %}

![](<../.gitbook/assets/Screenshot 2021-08-07 at 22.49.59.png>)

The protocol [takes fees](protocol-fees.md) for different operations, where a part goes to [Reserve Fund](liquidations/insurance-fund.md) and part to different protocol operations. All parameters and spending depend on [governance](../governance/setup/). Learn more:

{% content-ref url="protocol-fees.md" %}
[protocol-fees.md](protocol-fees.md)
{% endcontent-ref %}

***

## Modular Architecture

{% hint style="success" %}
Gearbox protocol has a modular architecture.&#x20;

The main logic is encapsulated in the core layer which supports operations for both protocol sides. It allows connecting customized pools with Credit Account managers without changing the internal codebase, and thus simplifying integrations.
{% endhint %}

The goal of Gearbox is to be integrated with existing and new protocols in an open-source manner and provide leverage across many user bases and products. Because of its modularity, leverage can be given to even long-tail assets without increasing passive lending side risks.

There could be segmentation of risks, personalized rates, collateral limits, and other mechanisms which allow modularity to shine and Gearbox to service different user groups. That could be farming, trading, sophisticated LP-ing, NFT and RWA leveraging, and so on.

<figure><img src="../.gitbook/assets/Gearbox Modular Architecture Intents.png" alt=""><figcaption></figcaption></figure>

See a more detailed developer explanation:

{% embed url="https://dev.gearbox.fi/credit/architecture" %}
