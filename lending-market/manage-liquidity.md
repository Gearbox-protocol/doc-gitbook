---
description: Earn APY in the same asset plus any additional GEAR APY or even other tokens.
---

# Dashboard: How to Earn

## Earning Passive APY

**Step 1.** Go to the [Passive Pools](https://app.gearbox.fi/pools) page. Click on the asset pool you want to earn with.

{% embed url="https://app.gearbox.fi/pools" %}

<figure><img src="../.gitbook/assets/Gearbox passive lending main dapp.png" alt=""><figcaption></figcaption></figure>

**Step 2.** Specify the amount you want to supply or just click on _MAX_.

<figure><img src="../.gitbook/assets/gearbox passive lending eth usdc dai wbtc.png" alt=""><figcaption></figcaption></figure>

**Step 3.** First, click _Approve_ and wait for the transaction to be confirmed. Then, click _Supply_ and wait for the confirmation. When a transaction is confirmed, you will receive (staked) [diesel tokens](pools-and-apy/#what-is-diesel-token).&#x20;

<figure><img src="../.gitbook/assets/gearbox passive lending supply approve.png" alt=""><figcaption></figcaption></figure>

{% hint style="success" %}
Done! Now you have (staked) [diesel tokens](pools-and-apy/#what-is-diesel-token). The organic APY from borrow and quota fees is being compounded into it, so there is nothing you need to do. Just sit back and relax.&#x20;
{% endhint %}

As for the GEAR or any other extra token yields, those are accruing to your staked dTokens too, but you need to claim them. _How often?_ - That's up to you to decide. You can claim the GEAR rewards either onchain via Etherscan, or simply click on the rewards tab in the top right corner of the interface.

### Extended View: Allowed Tokens

The V3 interface features an extended view. It helps you see what assets borrowers are trading and farming with. You don't necessarily need to care of this, because borrowers get liquidated in case their positions do not perform well - so the capital comes back to your pool anyway.

<figure><img src="../.gitbook/assets/gearbox extended dapp allowed tokens pools.png" alt=""><figcaption></figcaption></figure>

This transparency dashboard helps you better assess risks in different pools. For example, you can be comfortable that borrowers are leverage staking in Lido - but not comfortable that they are trading APE with leverage. As a result, if risk segmentation allows for it, you can choose a different pool to lend to. Or even better, you can stake the GEAR you earned to [vote in gauges](../governance/quotas-and-gauges/) and increase the rates APE traders are paying to you. This way, you improve your R/R because you bill them more!

* Vote on the quota limits and collateral limits being lower or higher with [main voting](../governance/setup/);
* Vote on the extra APY rates being lower or higher with [Gauges](../governance/quotas-and-gauges/).

{% hint style="info" %}
Conceptually, because Gearbox has a modular architecture, risks are isolated and are not shared across different pools. You can envision Gearbox with a totally personalized lender exposure down the line. If there will be demand for it, it can be done!
{% endhint %}

***

## Withdrawing liquidity

Do the same steps as above, but simply click on the "withdraw liquidity" tab in Step 2. Easy!

{% hint style="info" %}
If the utilization of the pool is too high, governance can increase the lend-borrow parameters and thereby make lending more expensive to incentivize repayments of lender capital. This will encourage borrowers to close loans and thereby reduce pool utilization.
{% endhint %}

{% hint style="warning" %}
Did you find a bug in the interface, something didn't work as you think it should have, or you have a suggestion on how to improve the user experience? - [Report on Discord](https://discord.gg/gearbox)!
{% endhint %}
