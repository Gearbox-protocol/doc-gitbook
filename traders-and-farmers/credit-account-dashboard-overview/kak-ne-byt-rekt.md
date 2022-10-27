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

1. **Add collateral**: the easiest method to improve your health factor is simply by adding more collateral in the form of the base asset that you opened your credit account in. If this isn't a possibility you can follow the below options.

<figure><img src="../../.gitbook/assets/Add more collateral.png" alt=""><figcaption></figcaption></figure>

&#x20;2\.  **Change strategy:** If you are in a strategy that has a directional trade that's leading to the HF dropping, a possible better idea could be to change to a strategy with stables or lesser volatile/base asset to preserve your credit account.

&#x20;3\.  **Decrease debt:** Add some of the collateral back to the CA in the form of the base asset you borrowed, this will help you lower your leverage and thus improve your health factor

&#x20;4\.  **Lower Leverage:** If the above isn't possible, you can close your leverage account and reopen it with a lower leverage level and this will ensure that while the value of your funds remains the same, the risk of liquidation is lower.

&#x20;5\.  **Close CA:** In the case where none of the above are beneficial, it makes more sense to close your credit account and preserve the funds you have instead of getting liquidated and losing it all.  &#x20;

{% content-ref url="how-to-close-account.md" %}
[how-to-close-account.md](how-to-close-account.md)
{% endcontent-ref %}

### Checking Health Factor of your Credit Account

In the [Credit Account's page](https://app.beta.gearbox.fi/accounts) you can check health factors of all your Credit Accounts:

<figure><img src="../../.gitbook/assets/screenshot-app-goerli-gearbox-fi-accounts-1666402061955.png" alt=""><figcaption></figcaption></figure>

Also you can check health factor inside the Credit Account:&#x20;

<figure><img src="../../.gitbook/assets/screenshot-app-goerli-gearbox-fi-accounts-0x2ad4a2f1bdd815e285a22cdcc072fbb-1666400881484 (3).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Anybody can run a liquidator bot and secure the protocol. You can chat about setting up your bot and other liquidator-things in [this Discord channel](https://discord.gg/wmydr8JfcP). Help users minimize the [risks](../../risk-and-security/risks-terms.md)!
{% endhint %}
