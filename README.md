---
description: Generalized Leverage Protocol ⚙ Built with composability in mind <3
---

# Overview&#x20;

![](.gitbook/assets/IMG\_7234.PNG)

Gearbox is a generalized leverage protocol. It has two sides to it: passive liquidity providers who earn low-risk APY by [providing single-asset liquidity](liquidity-providers/manage-liquidity.md); and active farmers or even other protocols who borrow those assets to [trade or farm with even x10 leverage](overview/credit-account/). See [how-it-works.md](overview/how-it-works.md "mention").

Gearbox Protocol allows anyone to take DeFi-native leverage and then use it across various (DeFi & more) protocols in a composable way. **You take leverage with Gearbox and then use it on other protocols you already love: Uniswap, Curve, Convex, Lido, etc.** For example, you can leverage trade on Uniswap, leverage farm on Yearn, make delta-neutral strategies, get Leverage-as-a-Service for your structured product, and more... Thanks to the [Credit Accounts](overview/credit-account/) primitive!

> Some compare composable leverage as a primitive to DeFi-native prime brokerage.
>
> The core vision is to become a backend **leverage middle layer**. You can envision building your own DeFi protocol and just making a “take leverage with Gearbox” as a button. And _bam_ - your users are now more capital efficient. Or integrate Gearbox into a platform like Zerion or Zapper. Check this page to understand why [composable leverage 2.0 is cool](leverage-2.0-is-composable.md)!

Developer docs can be found here:

{% content-ref url="https://app.gitbook.com/o/-MVf0w9QBIQw5nuscwFc/s/-MTW5vYjW5AmfzJsI9yS/" %}
[Gearbox Dev](https://app.gitbook.com/o/-MVf0w9QBIQw5nuscwFc/s/-MTW5vYjW5AmfzJsI9yS/)
{% endcontent-ref %}

### **Where is the DAO, how can I contribute?**

You can be in a DAO but not be 24/7 active, which is totally okay. There are different ways to get involved and get rewarded for your time and skills.&#x20;

* **Workers / core contributors**: those who day and/or night work on different tasks as core contributors, ranging from marketing to coding. DAO contributors are split among different sub-projects and can decide to work on something specific, or a few tasks at a time. [See Notion](https://gearboxprotocol.notion.site/Gearbox-DAO-23966f122ae4421492819242b30a0e7a).&#x20;
* **Delegates**: members who stay on top of protocol strategic ideas and plans, but don’t have the 24/7 to really get hands-on operational tasks. They can become delegates and lead how [governance](governance/setup/) decides on protocol vital things.&#x20;
* **Shitposters**: you can meme, learn, and discuss DeFi in [Discord](https://discord.com/invite/gearbox). We’ll like you ;) In fact, there is a _VIBES_ community program for the best posters, check it out [here](https://medium.com/gearbox-protocol/vibes-community-program-is-starting-welcome-to-the-1st-stage-e64a03f4c025).

{% embed url="https://gearboxprotocol.notion.site/gearboxprotocol/Gearbox-DAO-Working-Sheet-23966f122ae4421492819242b30a0e7a" %}

## **Cool Features**

* **Composable.** Gearbox does not have its own order book or trading environment. The leverage you get - is used across multiple DeFi protocols and assets, fully composable! For example, a yield aggregator can be on the liquidity provider side of Gearbox Protocol, as well as be an avenue for Gearbox users to deploy their leverage into. Learn [how-it-works.md](overview/how-it-works.md "mention").
* **0% Funding Rates**. The leverage offered is not based on derivative positions but is instead executed with real assets on third-party protocols. Because Gearbox does not create its own trading pairs, there is no short/long ratio that needs to be maintained with funding rates.&#x20;
* **Leverage as a Service.** Other protocols can offer leverage to their users with the help of Gearbox Protocol, without modifying anything in their own architecture. As such, they also get exposure to the user base of Gearbox. [Make a proposal to Gearbox DAO](https://gov.gearbox.fi/t/template-proposal-for-managing-gearbox-protocol-parameters/100)!
* **Permissionless Strategies.** Positions and trades within Credit Accounts can be extended to include complex strategies, for example, making a short position farm in Yearn; or having LP tokens as collateral for more composable actions.
* **Low overhead on gas.** Due to how data and operations are processed across isolated smart contracts, gas usage overhead is reduced to an insignificant overhead. [Learn more](overview/credit-account/#low-overhead-on-gas).

{% hint style="info" %}
With V2, Gearbox Protocol has become cooler & faster! It now has its own multicall for complex transactions, pathfinder for the best automated routing, integrations with Curve + Yearn + Convex + Lido, and more awesome stuff! Read here:
{% endhint %}

<> medium article link soon <>

### DAO-First Approach to Building

* **Decentralized.** CEXes subjectively define leverage parameters and also keep custody of your funds. With Gearbox, you are always in control of your funds. It's all transparent. There is no one EOA or team signature, it's all in the hands of [setup](governance/setup/ "mention").
* **Community-driven.** Gearbox Protocol does not have a company responsible for the protocol or on-chain actions. The goal is to make the protocol work based on how the community wants it.&#x20;
* You can check how from _day -1_ the focus has been on community-first [launch-phases](overview/launch-phases/ "mention").

{% embed url="https://gearboxprotocol.notion.site/gearboxprotocol/Gearbox-DAO-23966f122ae4421492819242b30a0e7a" %}
Notion pages set up to streamline DAO work and contributions.
{% endembed %}

MarketMake ETHGlobal 2021 hackathon finalist 🎆
