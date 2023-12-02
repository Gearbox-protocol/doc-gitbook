---
description: >-
  This page documents all the version upgrades that take place after the
  deployment of Gearbox V1 in Dec'21
---

# Subsequent Upgrades

## Gearbox V2

Gearbox V2 upgrade took place in October'22 and led to a $120M+ TVL increase. Post V1s usage, it became abundantly clear that the users are more interested in using Gearbox for Leveraged Farming than trading. V2 was thus born out of the effort to increase the avenues to leverage farm and provide a better user experience to the leverage farmers. With V2, the DAO expanded it's integrations with:

* Curve Pools
* Convex Pools
* Yearn Vaults&#x20;
* Lido Staking

This led to 14 more strategies becoming available to the users to leverage farm on. At the same time though, V1 required users to hop through multiple protocols to deploy a position. V2 was built with UX and ease of use in mind. This was brought on by:

1. **Multicall:** Multicall enabled users to open CA, perform required swaps, deploy in farm and receive LP tokens in a single transaction. While the farming happened natively on the integrated protocol, the need to leave Gearbox UI or click multiple buttons was removed.&#x20;
2. **Up to 10x Leverage:** V1 offered leverage up to 4x, this was upgraded by V2 with pools being able to offer as much as 10x leverage. This increased the max APYs a pool could produce significantly.&#x20;

The 2 factors together enabled V2 to bring leveraged farming to life. You can read more about it in the article below.

{% embed url="https://medium.com/gearbox-protocol/product-evolution-v2-gearbox-protocol-from-1-to-2-going-further-dcedf3b5d959" %}

***

## Gearbox V2.1&#x20;

Gearbox V2.1 was released in June'23, the update was largely focused on improving the security of the codebase. With DeFi exploits on the rise, it was crucial to upgrade and fortify the security of the codebase. Moreover, with V3 being built over the existing codebase, it enabled the DAO to battle test the V3 codebase even before it's deployment. It improved security 4 ways:

* Removed access mechanisms for adapters that had lower utility
* Introduced bad debt prevention parameters
* Identified and fixed possible existing bugs&#x20;
* Improved Account security at UI and operational level

You can read the complete details in the article below.

{% embed url="https://medium.com/gearbox-protocol/gearbox-pre-v3-redefine-security-e4a73b465cc8" %}

{% hint style="info" %}
Beyond these, the DAO is set to introduce Gearbox V3 in Q4. V3 will evolve Leverage Farming as per the [details shared](https://medium.com/gearbox-protocol/gearbox-v3-teaser-redefining-leverage-and-lending-ff62034e8a34?source=collection\_home---4------12-----------------------) and further also introduce Gearbox Spot Leverage Trading dApp. Spot Leverage will be the first app with non-synthetic perpetuals that don't require a house to trade against the user.
{% endhint %}
