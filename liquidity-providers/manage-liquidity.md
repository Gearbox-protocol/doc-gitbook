---
description: By providing liquidity, you can earn APY in the same asset. Simple!
---

# LP Dashboard - How to supply or withdraw liquidity

## Supplying liquidity

**Step 1.** Go to [Pools](https://app.beta.gearbox.fi/pools) page and click _Supply_ on the asset you want to supply.

![](<../.gitbook/assets/Screenshot 2021-10-17 at 14.11.00.png>)

**Step 2.** Specify the amount you want to supply or just click on _MAX_.

![](<../.gitbook/assets/Screenshot 2021-10-17 at 14.12.35.png>)

**Step 3.** First click _Approve_ and wait for the transaction to be confirmed. Then, click _Supply_ and wait for the confirmation. When a transaction is confirmed, you will receive [diesel tokens](pools-and-apy.md#what-is-diesel-token).&#x20;

![](<../.gitbook/assets/Screenshot 2021-10-17 at 14.14.09.png>)

## Withdrawing liquidity

**Step 1.** Go to [Pools](https://app.beta.gearbox.fi/pools) page and click _Withdraw_ on the asset you want to withdraw.

![](<../.gitbook/assets/Screenshot 2021-08-02 at 14.15.36.png>)

**Step 2.** Specify the amount you want to withdraw if you want to take out a bit or click _MAX_ if all.

![](<../.gitbook/assets/Screenshot 2021-10-17 at 14.18.09.png>)

**Step 3.** First click _Approve_ and wait for the transaction to be confirmed. Then click _Withdraw_ and wait for the confirmation. When a transaction is confirmed, you will receive back your assets.

{% hint style="warning" %}
Usually, in DeFi protocols forced liquidation is not implemented. This creates the risk of insufficient liquidity for the withdrawal operation. To mitigate this risk, the parameters for managing the interest rate curve of the pool are introduced (interest rate depends on utilization ratio of the pool). If the utilization of the pool is too high, governance can increase these parameters and thereby make lending more expensive. This will encourage borrowers to close loans and thereby reduce pool utilization.
{% endhint %}

{% hint style="info" %}
Did you find a bug with the interface, something didn't work as you think it should have, or you have a suggestion on how to improve the user experience? [Report](https://discord.gg/5YuHH9tvms) or [suggest](https://discord.gg/hF3QvX2vgt) on Discord!
{% endhint %}
