---
description: >-
  Stake and decide on the extra protocol fees. Quota Fees are established by the
  main governance process, while Gauges are fully onchain mechanisms that are
  for extra interest rates.
---

# Quotas and Gauges

## Quotas

Quotas are a mechanism that Gearbox V3 uses to track exposure to a particular collateral asset, both on the level of a single Credit Account, and on the level of the entire pool. A quota is the maximum underlying equivalent of a quoted asset that is counted towards collateral of a CA. This means that:

1. Quotas are denominated in units of underlying;
2. When computing the weighted value for a quoted asset, either the actual underlying-denominated value of the asset is used, or its quota - whichever is smaller.

See a proper technical explanation here:

{% embed url="https://dev.gearbox.fi/core/quota#quota-interest" %}

A quota is reserved by every leverage user themselves, “_how much of any X collateral asset on my Credit Account I want to go towards the total Health Factor_”. Probably, as much as possible. But anyway, see it as a technical implementation. It helps harmonize the distribution of limited collaterals between leverage users in a more democratic way, on the contract level.

{% hint style="success" %}
Quota Fees are decided by the main governance process, and are more or less static. They are taken every time you initially get or increase your quota for every asset. See in [Fees](../../overview/protocol-fees.md).
{% endhint %}

## G**auges**

<figure><img src="../../.gitbook/assets/GEAR fair yield distribution.jpeg" alt=""><figcaption></figcaption></figure>

Extra interest rate paid by borrowers are defined by Gauges on a per-epoch basis by GEAR stakers (similar to how Curve Gauge distributes CRV rewards depending on veCRV votes).

Gauges are basically a tool for “what extra APY rates on top of the usual utilization curve, for every asset separately, is being paid by a borrower every epoch” (an epoch is 7 days but could be longer). This is how the protocol bills extra for quotas, essentially.&#x20;

But **Gearbox gauges are not like inflationary gauges** in Curve, nono, quite the opposite.&#x20;

> Gauges are the instruments with which it is decided how much extra interest a borrower pays. GEAR stakers freeze their tokens and then vote. See how on the [Dashboard page](dashboard-gauge-voting.md).

Gauges interest rate change happens on a per epoch basis. After an epoch starts, this extra interest rate for users doesn’t change until next epoch, while voters can change their votes continuously.

{% hint style="success" %}
Gauges decide the extra APR a borrower pays for each asset. These rates are applied per-block like regular borrow rates. Voted by GEAR stakers onchain. See in [Fees](../../overview/protocol-fees.md).
{% endhint %}

These extra fees are accumulated in a [Fee Guard](../setup/guards-multisigs.md#fee-temporary-guard-5-10) and can be voted on to be distributed. Check the [Utility & Staking page](../../gear-token/utility-and-staking.md) to see more on how GEAR holders can vote on it.
