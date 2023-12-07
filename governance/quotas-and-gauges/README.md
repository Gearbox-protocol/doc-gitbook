---
description: Stake and decide on the extra protocol fees.
---

# Quotas and Gauges

## Quotas

Quotas are a mechanism that Gearbox V3 uses to track exposure to a particular collateral asset, both on the level of a single Credit Account, and on the level of the entire pool. A quota is the maximum underlying equivalent of a quoted asset that is counted towards collateral of a CA. This means that:

1. Quotas are denominated in units of underlying;
2. When computing the weighted value for a quoted asset, either the actual underlying-denominated value of the asset is used, or its quota - whichever is smaller.

See a proper technical explanation here:

{% embed url="https://dev.gearbox.fi/core/quota#quota-interest" %}

A quota is reserved by every leverage user themselves, “_how much of any X collateral asset on my Credit Account I want to go towards the total Health Factor_”. Probably, as much as possible. But anyway, see it as a technical implementation. It helps harmonize the distribution of limited collaterals between leverage users in a more democratic way, on the contract level.

An implementation of collateral limits basically.

<figure><img src="../../.gitbook/assets/GEAR fair yield distribution.jpeg" alt=""><figcaption></figcaption></figure>

## G**auges**

Interest rate paid by user for using quotas are defined by Gauges on a per-epoch basis by GEAR stakers (similar to how Curve Gauge distributes CRV rewards between different pools depending on veCRV votes). Gauges are basically a tool for “what extra APY rates on top of the usual utilization curve, for every asset separately, is being paid by a borrower every epoch” (an epoch is 7 days but could be longer). This is how the protocol bills extra for quotas, essentially.&#x20;

But **Gearbox gauges are not like inflationary gauges** in Curve, nono, quite the opposite.&#x20;

> Gauges are the instruments with which it is decided how much for every quota is paid. GEAR stakers freeze their tokens (against governance attacks) and then vote.

Quotas interest rate change happens on a per epoch basis - after epoch starts, quota interest rate for users doesn’t change until next epoch, while voters can change their votes continuously.

{% hint style="info" %}
These exra fees are accummulated in a [Fee Guard](../setup/guards-multisigs.md#fee-temporary-guard-5-10) and can be voted on to be distributed. Check the [Utility & Staking page](../../gear-token/utility-and-staking.md) to see more on how GEAR holders can vote on it.
{% endhint %}

{% content-ref url="../../overview/protocol-fees.md" %}
[protocol-fees.md](../../overview/protocol-fees.md)
{% endcontent-ref %}
