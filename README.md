---
description: Generalized Leverage Protocol ⚙ Built with composability in mind <3
---

# Overview&#x20;

![](.gitbook/assets/IMG\_7234.PNG)

Gearbox is a generalized leverage protocol. It has two sides to it: passive lenders who earn low-risk APY by lending[ single-asset](lending-market/manage-liquidity.md)s; and active farmers, firms, or even other protocols who borrow those assets to [trade or farm with even x10 leverage](overview/credit-account/). See [how-it-works.md](overview/how-it-works.md "mention").

Gearbox Protocol allows anyone to take DeFi-native leverage and then use it across various (DeFi & more) protocols. This enables you to compose your position as you want. **You take leverage with Gearbox and then use it on other protocols you already love: Uniswap, Curve, Convex, Lido**, etc. For example, you can leverage trade on Uniswap, leverage farm on Yearn, make delta-neutral strategies, hedge your exposure, get Leverage-as-a-Service for your structured product, and more... Thanks to the [Credit Accounts](overview/credit-account/) primitive!

> Some compare composable leverage as a primitive to DeFi-native prime brokerage.
>
> The core vision is to become a **leverage middle layer**. You can envision building your own DeFi protocol and just making a “take leverage with Gearbox” as a button. And _bam_ - your users are now more capital efficient. Or integrate Gearbox into a platform like Zerion or Zapper. Check this page to understand why [composable leverage 2.0 is cool](leverage-2.0-is-composable.md)!

**Developer docs can be found here:**

{% embed url="https://dev.gearbox.fi/" %}

### **Where is the DAO, how can I contribute?**

Gearbox is a DAO, run by various contributors and initiatives. The protocol and assets are never in custody of any one single person. You can be in a DAO but not be 24/7 active, which is totally okay. There are different ways to get involved and get rewarded for your time and skills. See more:

{% embed url="https://gearboxprotocol.notion.site/gearboxprotocol/Gearbox-DAO-Working-Sheet-23966f122ae4421492819242b30a0e7a" %}

<figure><img src=".gitbook/assets/IMG_0418.png" alt=""><figcaption><p><a href="https://gearboxprotocol.notion.site/Gearbox-DAO-23966f122ae4421492819242b30a0e7a"><strong>https://gearboxprotocol.notion.site/Gearbox-DAO-23966f122ae4421492819242b30a0e7a</strong></a></p></figcaption></figure>

## **Cool Features**

{% hint style="info" %}
With V2, Gearbox Protocol has become cooler & faster! It now has its own **new multicall** for complex transactions, **smart router** for the best automated routing of trades & deposits, **new integrations** with Curve + Yearn + Convex + Lido, and more:
{% endhint %}

{% embed url="https://medium.com/gearbox-protocol/product-evolution-v2-gearbox-protocol-from-1-to-2-going-further-dcedf3b5d959" %}

* **Composable.** Gearbox does not have its own order book or trading environment. The leverage you get - is used across multiple DeFi protocols and assets, fully composable! For example, a yield aggregator can be on the liquidity provider side of Gearbox Protocol, as well as be an avenue for Gearbox users to deploy their leverage into. Learn [how-it-works.md](overview/how-it-works.md "mention").
* **0% Funding Rates**. The leverage offered is not based on derivative positions but is instead executed with real assets on third-party protocols. Because Gearbox does not create its own trading pairs, there is no short/long ratio that needs to be maintained with funding rates.&#x20;
* **Leverage as a Service.** Other protocols can offer leverage to their users with the help of Gearbox Protocol, without modifying anything in their own architecture. As such, they also get exposure to the user base of Gearbox. [Make a proposal to Gearbox DAO](https://gov.gearbox.fi/t/template-proposal-for-managing-gearbox-protocol-parameters/100)!
* **Permissionless Strategies.** Positions and trades within Credit Accounts can be extended to include complex strategies, for example, making a short position farm in Yearn; or having LP tokens as collateral for more composable actions. In fact, you can make all of these complex things easier to ape into, by using Gearbox's unique multicall features.

### DAO-First Approach to Building

* **Decentralized.** CEXes subjectively define leverage parameters and also keep custody of your funds. With Gearbox, you are always in control of your funds. It's all transparent. There is no one EOA or team signature, it's all in the hands of [setup](governance/setup/ "mention").
* **Community-driven.** Gearbox Protocol does not have a company responsible for the protocol or on-chain actions. The goal is to make the protocol work based on how the community wants it.&#x20;
* You can check how from _day -1_ the focus has been on community-first [launch-phases](overview/launch-phases/ "mention").

_MarketMake ETHGlobal 2021 hackathon finalist_ 🎆
