---
description: The protocol takes fees for different operations.
---

# Protocol Fees

{% hint style="success" %}
1. All protocol fees that the DAO earns go to the [fee guard](../governance/setup/guards-multisigs.md#fee-temporary-guard-5-10). Nothing is assumed for the core contributors or the foundation. The protocol is fully operated by holders.
2. Because Gearbox is modular, fees are not protocol-wide. They can be different from one Credit Manager to another, depending on the liquidity of a given asset and type.
3. Most of the fees are static and are voted in via the [main governance process](../governance/setup/), however, [Quota fees with Gauges](../governance/quotas-and-gauges/) are voted on separately onchain every epoch.
{% endhint %}

### **Liquidation Fee**

_Goes only to the DAO._

If a Credit Account is liquidated, some percentage goes to a third-party liquidator who liquidated the account - and some percentage goes to Gearbox Protocol. These fees can vary from one Credit Manager to another, depending on how safe the margin for liquidation error should be.

* Current liquidation fee going to the liquidator: 4%
* Current liquidation fee going to the protocol: 1.5%

### APY Spread Fee

_Split between passive lenders and the DAO._

The protocol takes spread as a fee between the APY which lenders receive and the fee & farmers pay for borrowing their assets. The exact value of this fee is calculated as following:

* Each pool has it’s interest rate curve. This interest rate curve represents borrow APY that lenders receive as a function of pool’s utilization r(u). See details and formulas at [dev docs](https://dev.gearbox.fi/docs/documentation/pools/intro/#rt---borrow-apy).
* Borrowers pay borrow APY to liquidity providers and pay spread fee to DAO spreadFee. That means effective borrow rate for borrowers is calculated as r(u)\*(1+spreadFee). DAO receives r(u)\*spreadFee.

{% content-ref url="../lending-market/pools-and-apy/" %}
[pools-and-apy](../lending-market/pools-and-apy/)
{% endcontent-ref %}

### Trading Fee

_Goes only to the DAO._

This fee is similar to a trading fee, but not fully. It is taken when a borrower swaps any one asset to another. These fees are also different from one Credit Manager to another. For example, a 0.01% fee can be taken for an ETH long/short, while a 0.05% could be taken for more risky assets.

### Quota Fee from Gauges (Extra Borrow Rate)

_Split between passive lenders and the DAO._

Quota fees from gauges are basically an extra borrow rate applied to every different asset separately. It is taken per-block just like the regular borrow rate. This fee is voted on separately from the main DAO voting and is not static. It changes every epoch with gauges voted on by GEAR stakers.&#x20;

{% hint style="info" %}
For the exact math behind the fees and the split, see the Tech Paper page:
{% endhint %}

{% content-ref url="whitepaper.md" %}
[whitepaper.md](whitepaper.md)
{% endcontent-ref %}
