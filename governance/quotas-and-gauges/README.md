---
description: >-
  Stake and decide on protocol fees. Quota flat fees are established by the main
  governance process, while Gauges (extra Quota interest rates) are a fully
  onchain process.
---

# Quotas and Gauges

## Quotas (Limits)

> See them like individual collateral limits, applied per every Credit Account. In other words, it's like a credit line: you open it once for a fixed amount, and then it needs to change if you want to increase or decrease that credit line. Interfaces help you with that though!

Quotas are a mechanism that Gearbox V3 uses to track exposure to a particular collateral asset, both on the level of a single Credit Account, and on the level of the entire pool. A quota is the maximum underlying equivalent of a quoted asset that is counted towards collateral of a CA. This means that:

1. Quotas are denominated in units of underlying;
2. When computing the weighted value for a quoted asset, either the actual underlying-denominated value of the asset is used, or its quota - whichever is smaller.

See a proper technical explanation here:

{% embed url="https://dev.gearbox.fi/core/quota#quota-interest" %}

A quota is reserved by every leverage user themselves, “_how much of any X collateral asset on my Credit Account I want to go towards the total Health Factor_”. Probably, as much as possible. But anyway, see it as a technical implementation. It helps harmonize the distribution of limited collaterals between leverage users in a more democratic way, on the contract level.

{% hint style="success" %}
Quota Fees are decided by the main governance process, and are more or less static. They are taken every time you initially get or increase your quota for every asset. See in [Fees](../../overview/protocol-fees.md#quota-fee).
{% endhint %}

## G**auges (Extra Rates)**

**Gearbox gauges are not like inflationary gauges** in Curve - nonno, quite the opposite.&#x20;

> Gauges are the instruments with which it is decided how much extra quota interest rate a borrower pays. GEAR stakers freeze their tokens and then vote. See how on the [Dashboard page](dashboard-gauge-voting.md).

<figure><img src="../../.gitbook/assets/GEAR fair yield distribution.jpeg" alt=""><figcaption></figcaption></figure>

Extra quota interest rate paid by borrowers is defined by Gauges on a per-epoch basis by GEAR stakers (similar to how Curve Gauge distributes CRV rewards depending on veCRV votes). Gauges interest rate change happens on a per epoch basis. After an epoch starts, new rates for users don't change until the next epoch, meanwhile voters can change their votes continuously.

Gauges are basically a tool for _“what extra Quota APY rates on top of the usual utilization curve, for every asset separately, is being paid by a borrower”_ (an epoch is 7 days but could be longer). This is how the protocol bills extra for keeping riskier collaterals on a Credit Account, essentially.&#x20;

* Imagine you are a passive lender: you obviously want to earn a higher APY! So you will stake your GEAR and vote for increasing gauge rates for everything probably.
* Now imagine you are a leverage borrower. You want to pay less! So you will stake your GEAR and vote to decrease gauge rates for the specific assets you are utilizing.
* Now imagine you are a protocol integrated on Gearbox. You want more Leverage as a Service (have Gearbox borrowers enter your protocol). You will stake GEAR to vote and decrease the rates specifically for the assets relevant to your protocol, so your protocol becomes more attractive.&#x20;

{% hint style="success" %}
Gauges decide the extra APY a borrower pays for each asset. These rates are applied per-block like regular borrow rates. Voted by GEAR stakers onchain. See in [Fees](../../overview/protocol-fees.md).

**New epochs start every Monday at 12:00 UTC.**
{% endhint %}

These extra rates are split with passive lenders and are accumulated in the [Fee Guard](../setup/guards-multisigs.md#fee-temporary-guard-5-10). Check the [Utility & Staking page](../../gear-token/utility-and-staking.md) to see more about how GEAR holders can vote for these extra rates.
