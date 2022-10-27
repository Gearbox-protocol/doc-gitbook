---
description: A walk-through the main functions on Gearbox app interface.
---

# Inside a Credit Account

{% hint style="info" %}
Learn what a [Credit Account](../../overview/credit-account/) is and how it works.
{% endhint %}

### Operating a Credit Account

Post opening a credit account and taking a leverage position, you'll be able to see an interface that looks like the one below

<figure><img src="../../.gitbook/assets/screenshot-app-goerli-gearbox-fi-accounts-0x2ad4a2f1bdd815e285a22cdcc072fbb-1666402210046 (1).png" alt=""><figcaption></figcaption></figure>

There are 4 tabs inside a credit account that let you operate and utilise it to the max potential

1. **Trade:** This is where you can see the leveraged funds you have as well as swap them for a different asset. Swapping can affect your HF so take note of the same by monitoring the right side of the screen.&#x20;

{% content-ref url="trade-swapping-assets.md" %}
[trade-swapping-assets.md](trade-swapping-assets.md)
{% endcontent-ref %}

&#x20;2\.  **Farm:** Farm is where the real alpha lies. All the strategies for the biggest vaults and pools in DeFi that you want to ape into are available in farm without you having to hop protocol from protocol. You just need to select which pool/vault you want to go deploy in and done.&#x20;

<figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

&#x20;**** 3.  **Connect:** Connect is what enables you to use native adapters of the integrated protocols. You can use them if you like the familiarity but Single Click Strategies and the Farm option already have them available with way more convenience.&#x20;

{% content-ref url="connect-using-native-adapters.md" %}
[connect-using-native-adapters.md](connect-using-native-adapters.md)
{% endcontent-ref %}

&#x20;4\.  **Manage:** Manage tab let's you take multiple position management actions in order to help you take care of risk as well as to close your position. The options are listed below:

* **Borrow more:** If you have a great health score and feel borrowing more and upping the leverage is worth the play, you can use this feature to do the same.
* **Decrease Debt:** You can repay part of your debt to reduce your risk or to reduce the borrow fee you pay on your position.
* **Add collateral:** The easiest way to to improve your health score if your health score is getting close to liquidations level.
* **Close credit account:** The below page will help you manage the same.

{% content-ref url="how-to-close-account.md" %}
[how-to-close-account.md](how-to-close-account.md)
{% endcontent-ref %}

<figure><img src="../../.gitbook/assets/screenshot-app-goerli-gearbox-fi-accounts-0x2ad4a2f1bdd815e285a22cdcc072fbb-1666402365996.png" alt=""><figcaption></figcaption></figure>

While these are about the tabs for a credit account, there are certain parameters and values you need to take care of too. They are listed below.

### Account Parameters

At the top, you can see the balance of your Credit Account denominated in the underlying asset you opened your account in (it uses ChainLink oracle prices to calculate these values).

* **Health Factor** - your credit account can be liquidated if it falls below 1;
* **Total Value** - current balance of credit account, denominated in the underlying asset;
* **Customize** - choose a different look for the background of your Credit Account card**;**
* **Analytics** - check the stats of the pool and other charts in Gearbox-native analytics;
* **Etherscan** - see your Credit Account's address, and the assets / transactions.
* **Tokens** - the list of allowed tokens as per the policy which you can trade among.

<figure><img src="../../.gitbook/assets/screenshot-app-goerli-gearbox-fi-accounts-0x2ad4a2f1bdd815e285a22cdcc072fbb-1666400881484 (2).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Did you find a bug with the interface, something didn't work as you think it should have, or you have a suggestion on how to improve the user experience? [Report](https://discord.gg/5YuHH9tvms) or [suggest](https://discord.gg/hF3QvX2vgt) on Discord!
{% endhint %}
