---
description: Generalized Leverage Protocol ⚙ With composability in mind <3
---

# Overview&#x20;

![](.gitbook/assets/IMG\_7234.PNG)

Gearbox is a generalized leverage protocol: it allows you to take leverage in one place and then use it across various DeFi protocols and platforms in a composable way. The protocol has two sides to it: passive liquidity providers who earn higher APY by [providing liquidity](liquidity-providers/manage-liquidity.md); active traders, farmers, or even other protocols who can borrow those assets to [trade or farm with x4+ leverage](broken-reference).

The core vision is to become a backend **composable leverage protocol** that all kinds of users have but don’t even need to interact directly with any interface. You can envision building your own DeFi protocol and just making a “take leverage with Gearbox” as a button. And _bam_ - your users are now more capital efficient. Or integrate Gearbox into a platform like Zerion or Zapper.

Developer docs can be found here:

{% content-ref url="https://app.gitbook.com/o/-MVf0w9QBIQw5nuscwFc/s/-MTW5vYjW5AmfzJsI9yS/" %}
[Gearbox Dev](https://app.gitbook.com/o/-MVf0w9QBIQw5nuscwFc/s/-MTW5vYjW5AmfzJsI9yS/)
{% endcontent-ref %}

**Join the DAO and become one of the contributors:**

{% embed url="https://gearboxprotocol.notion.site/gearboxprotocol/Gearbox-DAO-Working-Sheet-23966f122ae4421492819242b30a0e7a" %}

## **Cool Features**

* **Composable.** Gearbox does not have its own order book or trading environment. The leverage you get is used across multiple DeFi protocols and assets, fully composable! For example, a yield aggregator can be on the liquidity provider side of Gearbox Protocol, as well as be an avenue for Gearbox users to deploy their leverage into. Learn [how Gearbox works](overview/how-it-works.md#core-pieces-in-gearbox-protocol).
* **0% Funding Rates**. The leverage offered is not based on synthetic positions but instead is executed with real assets on third-party protocols. Because Gearbox does not create its own trading pairs, there is no short-long ratio that needs to be maintained with funding rates.&#x20;
* **Leverage as a Service.** Other protocols can offer leverage to their users with the help of Gearbox Protocol, without modifying anything in their own architecture. As such, they also get exposure to the user base of Gearbox. [Make a proposal to Gearbox DAO](https://gov.gearbox.fi/t/template-proposal-for-managing-gearbox-protocol-parameters/100)!
* **Permissionless Strategies.** Positions and trades within Credit Accounts can be extended to include complex strategies, for example, making a short position farm in Yearn; or having LP tokens as collateral for more composable actions.
* **Low overhead on gas.** Due to how data and operations are processed across isolated smart contracts, gas usage overhead is reduced to an insignificant overhead. [Learn more](overview/credit-account/#low-overhead-on-gas).

#### DAO-First Approach to Building

* **Decentralized.** CEXes subjectively define leverage parameters and also keep custody of your funds. With Gearbox, you are always in control of your funds. It's all transparent. There is no one EOA or team signature, it's all in the hands of [governance](governance/setup/).
* **Community-driven.** Gearbox Protocol does not have a company responsible for the protocol or on-chain actions. The goal is to make the protocol work based on how the community wants it.&#x20;
* You can check how from day -1 the focus has been on community-first and DAO-driven [here](overview/launch-phases/#dao-taking-over-december-2021).

## Useful Links

* **Join** **Discord** 👾 [https://discord.com/invite/gearbox](https://discord.com/invite/gearbox)&#x20;
* Website: [https://gearbox.fi/](https://gearbox.fi)&#x20;
* Dev docs: [https://dev.gearbox.fi/](https://dev.gearbox.fi)
* Mainnet dApp: [https://app.gearbox.fi/ ](https://app.gearbox.fi)
* Kovan dApp: [https://app.kovan.gearbox.fi/](https://app.kovan.gearbox.fi/accounts)
* Developer Docs: [https://dev.gearbox.fi/](https://dev.gearbox.fi)
* Forum: [https://gov.gearbox.fi/t/start-here-forum-rules/](https://gov.gearbox.fi/t/start-here-forum-rules/)
* Blog Medium: [https://medium.com/@gearboxprotocol](https://medium.com/@gearboxprotocol)
* Github: [https://github.com/Gearbox-protocol](https://github.com/Gearbox-protocol)
* Twitter: [https://twitter.com/GearboxProtocol](https://twitter.com/GearboxProtocol)
* Snapshot page: [https://snapshot.org/#/gearbox.eth](https://snapshot.org/#/gearbox.eth)
* Deployed Contracts: [https://dev.gearbox.fi/contracts/deployed-contracts](https://dev.gearbox.fi/contracts/deployed-contracts)
* DAO To-Do Working Notion:&#x20;

{% embed url="https://gearboxprotocol.notion.site/gearboxprotocol/Gearbox-DAO-23966f122ae4421492819242b30a0e7a" %}
Notion pages set up to streamline DAO work and contributions.
{% endembed %}

MarketMake ETHGlobal 2021 hackathon finalist 🎆
