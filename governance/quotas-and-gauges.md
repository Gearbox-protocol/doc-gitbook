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

A quota is reserved by every leverage user themselves, “_how much of any X collateral asset on my Credit Account I want to go towards the total Health Factor_”. Obviously, as much as possible. But anyway, see it as a technical implementation. It helps harmonize the distribution of limited collaterals between leverage users in a more democratic way, on the contract level.

As a leverage user, you essentially borrow a debt asset (say USDC) and specify what it goes into: a trade, a farm or whatever. As a result, the protocol is able to know how much extra to bill you depending on whether you are in a risky asset or not… It happens seamlessly!

## G**auges**

<figure><img src="../.gitbook/assets/GEAR Gauges Quotas.png" alt=""><figcaption></figcaption></figure>

These are not like inflationary gauges in Curve, nono, quite the opposite.&#x20;

Gauges are basically a tool for “what extra APY rates on top of the usual utilization curve, for every asset separately, is being paid by a borrower every epoch” (an epoch is 7 days but could be longer). This is how the protocol bills extra for quotas, essentially.&#x20;

> Gauges are the instruments with which it is decided how much for every quota is paid. GEAR stakers freeze their tokens (against governance attacks) and then vote.

<figure><img src="../.gitbook/assets/GEAR fair yield distribution.jpeg" alt=""><figcaption></figcaption></figure>
