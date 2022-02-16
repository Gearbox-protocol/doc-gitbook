---
description: Don't fall prey to the liquidation bots and protect your funds!
---

# How to avoid liquidations

Liquidations are there to protect the liquidity providers' capital which by default shouldn't be exposed to directional risk which traders and farmers take. As a trader or farmer - you can avoid liquidations which keeps the protocol more healthy, as well as avoid the [fees](../../overview/protocol-fees.md) paid to liquidators & the protocol.

{% content-ref url="../../overview/liquidations/" %}
[liquidations](../../overview/liquidations/)
{% endcontent-ref %}

[Health Factor ](../../overview/liquidations/#what-is-a-health-factor)is the representation of your Credit Account's performance. Keep it high enough, and it should generally be fine - unless a major market event comes where your positions could go down 25% or more in a matter of minutes. The health factor should technically be above 1, however, any small market movement could liquidate you if the HF is too low. Make sure to keep it high and watch out!

{% hint style="info" %}
Keep your health factor as high as possible. Make sure it doesn't drop close to 1.
{% endhint %}

### What I can do if my health factor is close to 1 to keep my Credit Account alive?&#x20;

One of the ways is to add more collateral and thus improving the HF:

{% content-ref url="how-to-add-a-collateral.md" %}
[how-to-add-a-collateral.md](how-to-add-a-collateral.md)
{% endcontent-ref %}

You can also close your Credit Account if you want to cut the losses and avoid full annihilation:

{% content-ref url="how-to-close-account.md" %}
[how-to-close-account.md](how-to-close-account.md)
{% endcontent-ref %}

### Checking Health Factor of your Credit Account

In the [Credit Account's page](https://app.beta.gearbox.fi/accounts) you can check health factors of all your Credit Accounts:

![](<../../.gitbook/assets/Screenshot 2021-10-17 at 23.53.05 (1).png>)

Also you can check health factor inside the Credit Account:&#x20;

![](<../../.gitbook/assets/Screenshot 2021-10-17 at 14.26.47.png>)

{% hint style="info" %}
Anybody can run a liquidator bot and secure the protocol. You can chat about setting up your bot and other liquidator-things in [this Discord channel](https://discord.gg/wmydr8JfcP). Help users minimize the [risks](../../risk-and-security/risks-terms.md)!
{% endhint %}
