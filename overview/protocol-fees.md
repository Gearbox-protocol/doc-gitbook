---
description: The protocol takes fees for different operations.
---

# Protocol Fees

{% hint style="success" %}
1. All protocol fees that DAO earns go to the [fee guard](../governance/setup/guards-multisigs.md#fee-temporary-guard-5-10). Nothing is assumed for the core contributors or the foundation. The protocol is fully operated by holders. The fees, collected in dTokens, automatically become a [Reserve Fund unless unwrapped](liquidations/insurance-fund.md).
2. Because Gearbox is modular, fees are not the same everywhere. They can be different from one Credit Manager to another, depending on the type of a given asset.
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

### Quota Fee

_Goes only to the DAO._

This fee is similar to a trading fee, but not fully. It is applied whenever you buy a quota. These fees are also different from one Credit Manager to another. For example, a 0.01% fee can be taken for an ETH long/short, while a 0.03% could be taken for more risky assets. Here is how it works:

* Let's say, you open a position where you end up with $500,000 worth of ETH long or an ETH farm token, for example, [leverage staking](../traders-and-farmers/strategies/leveraged-liquid-staking.md). As such, you pay that specific fee on the entry into this position (buying a quota for it). For example, at 0.01% that is just $50.
* Then, you don't trade into anything but that $500K position grows in value and you want to make sure its bigger size (the surplus) is counted towards Health Factor. Let's say it appreciated by $100K. You pay only on that $100K difference. That would be $10 in this case.
* You decide to trade that $500K worth of whatever into another asset of the same position size. As such, you pay another specific fee for entering into a different asset. Let's say that asset's quota fee is 0.03%. That means you would pay $150 in this case.

{% hint style="info" %}
That is why you can kind of see it as a trading fee, but the second example provided above shows that it's not always about trading. It's about "buying quota allocation".
{% endhint %}

### Gauges: Extra Borrow Rate

_Split between passive lenders and the DAO._

Gauges are basically an extra borrow rate applied to every different asset separately. It is taken per-block just like the regular borrow rate. This fee is voted on separately from the main DAO voting and is not static. It changes every epoch with gauges voted on by GEAR stakers:

{% content-ref url="../governance/quotas-and-gauges/" %}
[quotas-and-gauges](../governance/quotas-and-gauges/)
{% endcontent-ref %}

<figure><img src="../.gitbook/assets/GEAR Gauges Quotas.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
For the exact math behind the fees and the split, see the Tech Paper page:
{% endhint %}

{% content-ref url="whitepaper.md" %}
[whitepaper.md](whitepaper.md)
{% endcontent-ref %}
