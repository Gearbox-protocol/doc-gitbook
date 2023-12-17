---
description: The protocol takes fees for different operations.
---

# Protocol Fees

{% hint style="success" %}
1. All protocol fees that DAO earns go to the [fee guard](../governance/setup/guards-multisigs.md#fee-temporary-guard-5-10). Nothing is assumed for the core contributors or the foundation. The protocol is fully operated by holders. The fees, collected in dTokens, automatically become a [Reserve Fund unless unwrapped](liquidations/insurance-fund.md).
2. Because Gearbox is modular, fees are not the same everywhere. They can be different from one Credit Manager to another, depending on the type of a given asset.
3. Most of the fees are static and are voted in via the [main governance process](../governance/setup/), however, [Gauges](../governance/quotas-and-gauges/) are voted on separately onchain every epoch.
{% endhint %}

### **Liquidation Fee**

_Goes only to the DAO._

If a Credit Account is liquidated, some percentage goes to a third-party liquidator who liquidated the account - and some percentage goes to Gearbox Protocol. These fees can vary from one Credit Manager to another, depending on how safe the margin for liquidation error should be.

* Fee going to the liquidator: 4%
* Fee going to the protocol: 1.5%

<figure><img src="../.gitbook/assets/Screenshot 2023-12-08 at 11.40.56.png" alt=""><figcaption></figcaption></figure>

### APY Spread Fee

_Split between passive lenders and the DAO._

The protocol takes spread as a fee between the APY which lenders receive and the fee & farmers pay for borrowing their assets. The exact value of this fee is calculated as following:

* Each pool has it’s interest rate curve. This interest rate curve represents borrow APY that lenders receive as a function of pool’s utilization r(u). See details and formulas at [dev docs](https://dev.gearbox.fi/docs/documentation/pools/intro/#rt---borrow-apy).
* Borrowers pay borrow APY to liquidity providers and pay spread fee to DAO spreadFee. That means effective borrow rate for borrowers is calculated as r(u)\*(1+spreadFee). DAO receives r(u)\*spreadFee.

<figure><img src="../.gitbook/assets/Screenshot 2023-12-08 at 11.51.40.png" alt=""><figcaption></figcaption></figure>

### Gauges: Extra APY Rate

_Split between passive lenders and the DAO._

Gauges are basically an extra interest rate applied to every different asset separately. It is taken per-block just like the regular interest rate. This rate is voted on separately from the main DAO voting and is not static. It changes every epoch with gauges voted on by GEAR stakers:

{% content-ref url="../governance/quotas-and-gauges/" %}
[quotas-and-gauges](../governance/quotas-and-gauges/)
{% endcontent-ref %}

<figure><img src="../.gitbook/assets/Screenshot 2023-12-08 at 12.11.26.png" alt=""><figcaption></figcaption></figure>

### Quota Fee

_Goes only to the DAO._

This fee is similar to a trading fee, but not fully. It is applied whenever you buy a quota. That can when entering a position for the first time, rebalancing (trading) into different assets inside the already open position, or when increasing your leverage or borrowing power.&#x20;

These fees are also different from one Credit Manager to another. For example, a 0.01% fee can be taken for an ETH long/short, while a 0.03% could be taken for more risky assets. Here is how it works:

* Let's say, you open a position where you end up with $100,000 worth of ETH long or an ETH farm token, for example, [leverage staking](../traders-and-farmers/strategies/leveraged-liquid-staking.md). As such, you pay that specific fee on the entry into this position (buying a quota for it). For example, at 0.01% that is just $10.

<figure><img src="../.gitbook/assets/Screenshot 2023-12-08 at 12.00.12.png" alt=""><figcaption></figcaption></figure>

* Then, you don't trade into anything but that $100K position grows in value and you want to make sure its bigger size (the surplus) is counted towards Health Factor. Let's say it appreciated by $10K. You pay only on that $10K difference. That would be $1 in this case.
* Alternatively, you decide to trade a part of that $100K into different assets of the same position size. As such, you pay another specific fee for entering into every different asset. Let's say those assets' quota fees are 0.03% and 0.05%. That means you pay $26 in this case.

<figure><img src="../.gitbook/assets/Screenshot 2023-12-08 at 12.09.50.png" alt=""><figcaption></figcaption></figure>

That is why you can kind of see it as a trading fee, but the second example provided above shows that it's not always about trading. **It's about "buying quota allocation".**

{% hint style="info" %}
For the exact math behind the fees and the split, see Tech Paper:
{% endhint %}

{% content-ref url="whitepaper.md" %}
[whitepaper.md](whitepaper.md)
{% endcontent-ref %}
