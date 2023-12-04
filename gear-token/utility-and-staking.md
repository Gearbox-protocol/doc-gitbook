---
description: Staking and utility sinks that exist for GEAR.
---

# Utility & Staking

GEAR token is an ERC20 utility token, starting off as a governance token for the protocol - and then possibly taking any other new function the DAO could envision for it. [Supply information is here](supply-information.md).

Currently, it seems that GEAR has a few different ways to be used, and those can expand.

***

### Main DAO Governance: Snapshot

Directing protocol treasury and grants, voting on parameters, onboarding assets and protocols, and so on. That happens on snapshot, see how on [governance page](../governance/setup/). You can vote on proposals or propose yourself even if you don't hold idle GEAR but have them in the GEAR-ETH Curve LP. Then your GEAR is taken into account, for [delegation](../governance/community-delegates.md) as well. Snapshot can expand its "strategies" to also account for [Quotas & Gauges](utility-and-staking.md#quotas-and-gauges) balances of stakers, and so on. It's configurable.

{% content-ref url="../governance/setup/" %}
[setup](../governance/setup/)
{% endcontent-ref %}

### Quotas and Gauges

GEAR stakers can freeze their tokens for 28 days and vote on the extra rates borrowers are paying for every different asset. This is a very important protocol function, because it (1) creates better and more fair rate markets whereas (2) this extra fee is split between passive lenders to compensate them for their liquidity as well as the DAO (the fee goes into the [separate fee multisig](../governance/setup/guards-multisigs.md#fee-temporary-guard-5-10)).&#x20;

{% content-ref url="../governance/quotas-and-gauges.md" %}
[quotas-and-gauges.md](../governance/quotas-and-gauges.md)
{% endcontent-ref %}

{% hint style="success" %}
It is logical to expect that some of these utilities and staking contracts should be harmonized, so holders could do a few things at a time. Should it be? How? Should the LM move over from Curve to Uniswap? [Discuss these ideas and propose your solution](https://discord.com/channels/841203475606011905/1177177691842166844).
{% endhint %}

### GEAR-ETH Curve Pool

There is liquidity mining ongoing for the[ GEAR-ETH pair on Curve V2](https://curve.fi/#/ethereum/pools/factory-crypto-192/deposit). You take some impermanent loss on it potentially, but get an APR at the rate that might compensate for that and above. The rewards in GEAR accrued you need to claim yourself automatically, or go to Convex / Yearn for this.

Make sure to "Deposit & Stake" your Curve LP tokens, as their interface suggests.

<figure><img src="../.gitbook/assets/GEAR token Curve.png" alt=""><figcaption><p><a href="https://curve.fi/#/ethereum/pools/factory-crypto-192/deposit">https://curve.fi/#/ethereum/pools/factory-crypto-192/deposit</a></p></figcaption></figure>

#### Others

There could be anyone offering utility sinks for GEAR. It's up to every holder individually to decide which of the utility sinks they want to engage in. You can also propose and / or make your own staking contract, or propose to the DAO to offer something else. [Jump in Discord](https://discord.gg/gearbox) for that!
