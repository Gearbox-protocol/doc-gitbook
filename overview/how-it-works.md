---
description: High-level technical overview of Gearbox Protocol.
---

# How it works

Gearbox protocol has two sides to it:

* **Lenders** - **liquidity providers** who seek passive yield and prefer lower risks. This can be seen similar to providing liquidity to Compound and getting cTokens back. LPs' assets are utilized by others, for which they get APY. Any one can be a liquidity provider on Gearbox.
* **Borrowers** - **traders, farmers, and protocols** who wish to increase their position by borrowing liquidity from the protocol at multiples of their collateral, for which they pay interest rates. The liquidity they borrow can be 10x of what their notional size is. This is the leverage power!

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

## Core parts of Gearbox Protocol

<figure><img src="../.gitbook/assets/Screenshot 2021-08-07 at 22.53.18.png" alt=""><figcaption></figcaption></figure>

One of the key aspects which actually makes this DeFi primitive possible are [Credit Accounts](credit-account/) (and Credit Managers), which “bind” together lenders and borrowers in this equation. More specifically, a Credit Account is an isolated smart contract that holds user + borrowed funds, has liquidation thresholds, and **has a list of** [**allowed tokens and protocols**](credit-account/#allowed-list-policy) (in order to avoid attack vectors from malicious actors, like borrowing leverage and buying a self-created ERC20 token; or sending an amount to a malicious smart contract).

{% content-ref url="credit-account/" %}
[credit-account](credit-account/)
{% endcontent-ref %}

**Gearbox does not silo the assets within its protocol.**&#x20;

All trades and operations happen on third-party protocols: Uniswap, Curve, Yearn, etc. **Your assets never end up in custody of any one person or company**. As such, Gearbox Protocol is not a trading platform / protocol. The protocol does not have its own order books, or control the secondary market liquidity. Therefore, there are no funding rates.

Integrations possibilities are very broad, as Gearbox is built with composability at its core:

{% content-ref url="integrations.md" %}
[integrations.md](integrations.md)
{% endcontent-ref %}

The positions which traders and farmers take should be liquidated by third-party [liquidators](liquidations/) before the assets of liquidity providers would start being exposed to the downside. As such, the protocol returns the liquidity providers’ assets to the pools if all functions correctly and liquidators do their job. This is how Gearbox is able to provide composable leverage.&#x20;

The liquidations are based on the **health factor and the threshold weighted value**:

{% content-ref url="liquidations/" %}
[liquidations](liquidations/)
{% endcontent-ref %}

![](<../.gitbook/assets/Screenshot 2021-08-07 at 22.49.59.png>)

The protocol [takes fees](protocol-fees.md) for different operations, where a part goes to [Reserve Fund](liquidations/insurance-fund.md) and part to different protocol operations. All parameters and spending depend on the [governance](../governance/setup/). Learn more:

{% content-ref url="protocol-fees.md" %}
[protocol-fees.md](protocol-fees.md)
{% endcontent-ref %}
