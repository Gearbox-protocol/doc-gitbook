---
description: Offering leverage to your users with Gearbox, or fully integrate.
---

# Integrations

{% hint style="info" %}
See [dev docs](https://dev.gearbox.fi/) or technical documentation and guidance:
{% endhint %}

{% embed url="https://dev.gearbox.fi/" %}

List of currently integrated protocols by Gearbox DAO:

{% content-ref url="credit-account/allowedlist-policy.md" %}
[allowedlist-policy.md](credit-account/allowedlist-policy.md)
{% endcontent-ref %}

Gearbox protocol has a flexible, adaptable, and scalable architecture.&#x20;

The main business logic is encapsulated in the core layer which supports operations for both protocol sides. It allows connecting customized pools with Credit Account managers without changing the internal codebase, and thus simplifying the integration process.

The goal of Gearbox is to be integrated with existing and new protocols in an open-source manner and provide leverage across many user bases. The architecture allows integration on both sides: both by protocols that are interested in granting leveraged access to their operations as well as by protocols that could provide supply-side lending liquidity like Aave, Compound, Iron Bank, etc.

{% embed url="https://github.com/Gearbox-protocol" %}

## How to integrate on a contract level

The integration process looks pretty simple: it is required to inherit an abstract contract (Credit Account Manager or Pool) and add specific business logic with set parameters. To be integrated with deployed contracts, the integration should be approved by Gearbox [governance](../governance/setup/).

Simple integration processes open up new opportunities for collaborations with other protocols, providing leverage to their operations and making Gearbox protocol composable. Overall, Gearbox aims to increase capital efficiency in the DeFi space.&#x20;

For more details, please ask the community on [Discord](https://discord.gg/JZgvmaenwn). Template proposal to Gearbox DAO:

{% embed url="https://gov.gearbox.fi/t/template-proposal-for-managing-gearbox-protocol-parameters/100" %}

## How to integrate your interface application

Gearbox core vision is that users should continue to use the DeFi protocols they love, but ... with leverage. Keeping this goal in mind, we have implemented a special library that makes it possible for any dApp to be connected with Gearbox credit account in a similar way to how Metamask or Fortmatic work. See more in the Developer Docs:

{% embed url="https://dev.gearbox.fi/" %}
