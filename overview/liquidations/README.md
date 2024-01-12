---
description: Defining liquidations, health factor, and weighted thresholds.
---

# Liquidations

#### How does the protocol ensure over-collaterization while allowing users leveraged operations?

When trading with Gearbox, your [Credit Account](../credit-account/) becomes the collateral for external protocols/actions: both your initial funds and the borrowed amount you got from the protocol. Gearbox Protocol sees which tokens your portfolio consists of and can determine its value at all times, which are always calculated in the underlying borrowed asset which you opened that Credit Account in.&#x20;

Gearbox uses a risk model to continuously assess the quality-value of a Credit Account. For each Credit Account, it computes its health factor**.**&#x20;

Anyone can check the health factor and liquidate positions with a health factor less than 1.

![](<../../.gitbook/assets/Screenshot 2021-10-18 at 21.48.21.png>)

{% hint style="warning" %}
As a user with a leverage position, you need to watch out for your health factor. Having it just above 1 puts you in risk of getting liquidated. Learn how to avoid liquidations.&#x20;
{% endhint %}

{% content-ref url="../../traders-and-farmers/credit-account-dashboard-overview/kak-ne-byt-rekt.md" %}
[kak-ne-byt-rekt.md](../../traders-and-farmers/credit-account-dashboard-overview/kak-ne-byt-rekt.md)
{% endcontent-ref %}

Learn about the current fee model a user pays in case of a liquidation:

{% content-ref url="../protocol-fees.md" %}
[protocol-fees.md](../protocol-fees.md)
{% endcontent-ref %}

### What is a Health Factor?

Health Factor is a numeric representation of your account health. If your health factor drops below 1 or close to it, you might be liquidated. The higher the number is, the safer you are. There are some tips on how you can avoid liquidations, [check them here](../../traders-and-farmers/credit-account-dashboard-overview/kak-ne-byt-rekt.md).

$$
H_{f}(t) =\frac{TWV(t)}{b(t) +interest\;accrued(t)},
$$

where _b(t)_ is borrowed amount.&#x20;

Let's dive into some math formulas to clarify how computation of the health factor works.&#x20;

### Total Value&#x20;

Represents the Credit Account's balance in the underlying asset.&#x20;

$$
TV(t)=\sum{\;c_i(t)*p_i(t)},
$$

where c\_i - balance of i-th asset in credit account,  p\_i - price of i-th asset calculated in underlying asset(from ChainLink oracle).

### Threshold Weighted Value&#x20;

$$
TWV(t)=\sum{min(Q_i(t),\;c_i(t)*p_i(t)*LT_i) }
$$

where: \
Q\_i - Quota amount for i-th asset in Credit Account (see [quotas-and-gauges](../../governance/quotas-and-gauges/ "mention")section),

c\_i - balance of i-th asset in credit account, \
p\_i - price of i-th asset calculated in underlying asset(from ChainLink oracle), \
LT\_i - liquidation threshold, the credit account manager constant showing the maximum allowable ratio of [Loan-To-Value](https://www.investopedia.com/terms/l/loantovalue.asp) for the i-th asset**.**&#x20;

### Liquidation Threshold

Liquidation thresholds represents maximum allowable ratio of Loan-To-Value for the i-th asset (LTV is reciprocal of over-collaterization ratio of i-th asset). LT\_i for underlying asset is constant and equals:

$$
LT_U =100\% - Liquidation\;Premium -Liquidation\;Fee
$$

**How is Liquidation Threshold defined?**

Gearbox Protocol uses statistics of 5-min, 15-min, 1h change of i-th asset's price (price is in the underlying asset) for the last 180 days.&#x20;

{% hint style="info" %}
Anybody can run a liquidator bot and secure the protocol. You can chat about setting up your bot and other liquidator-things in [Discord](https://discord.gg/wmydr8JfcP).
{% endhint %}
