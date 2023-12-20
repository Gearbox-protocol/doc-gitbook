---
description: A walk-through the main functions on Gearbox app interface.
---

# Tips for leverage users

{% hint style="info" %}
Learn [how to open a Credit Account](../how-to-open-account.md) if you have not done it yet.
{% endhint %}

### Operating a Credit Account: Leverage Farming

Post opening a Credit Account and taking a leverage position, you'll be able to see an interface that looks like the one below:

<figure><img src="../../.gitbook/assets/Dashboard (1).png" alt=""><figcaption></figcaption></figure>

There are 4 tabs inside a Credit Account that let you operate and utilise it to the max potential.

1. **Swap:** This is where you can see the leveraged funds you have as well as swap them for a different assets. Swapping can affect your HF so take note of the same by monitoring the right side of the screen. Usually, the interface would give a preview of your HF change.
2. **Farm:** Farm is where the real alpha lies. It shows all the strategies that you already are in. And all the strategies for the biggest vaults and pools in DeFi that you could ape into are available in farm without you having to hop protocol from protocol. You just need to select which pool/vault you want to go deploy in, and done.&#x20;

<figure><img src="../../.gitbook/assets/Farm page.png" alt=""><figcaption></figcaption></figure>

&#x20;3\.  **Manage:** Manage tab lets you take multiple position management actions in order to help you take care of risk as well as to close your position. The options are listed below:

<figure><img src="../../.gitbook/assets/Farm plain.png" alt=""><figcaption></figcaption></figure>

* **Quota Management:** Whether you want to increase the size of your position or want more of your assets to contribute towards your Health Factor, increasing quotas should help you. If you want to reduce the size of your position and don't want to pay Quota Interest on non-utilised value, decreasing Quotas should do the job. Just make sure you have enough Quota value contributing to your HF above your position size.
* **Borrow more:** If you have good Health Factor and feel like borrowing more and upping the leverage is worth the play - you can use this feature.
* **Decrease Debt:** You can repay part of your debt to reduce your risk or to reduce the borrow fee you pay on the capital you borrow.
* **Add collateral:** The easiest way to to improve your Health Factor if your Health Factor is getting close to liquidations level, which is < 1.
* **Close Credit Account:** The below page will help you manage the same.

4. **Agents:** Agents are Gearbots that enable you to automate operations on your CA. This makes features like Limit Order, DCA, Stop Loss and more possible without you actively managing the account at all times. These should come out with V1 of PURE, more on these then.

{% content-ref url="how-to-close-account.md" %}
[how-to-close-account.md](how-to-close-account.md)
{% endcontent-ref %}

***

## Operating a Credit Account: Margin Trading

Similar to Leverage Farming, Margin Trading interface has options to manage your trading operations too

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

Choose the position you want to manage and click on the menu option next to the close button. Doing so should take you the Manage Menu of the selected position

<figure><img src="../../.gitbook/assets/Leverage plain (1).png" alt=""><figcaption></figcaption></figure>

* **Borrow more:** If you have good Health Factor and feel like borrowing more and upping the leverage is worth the play - you can use this feature.
* **Borrow Less:** You can repay part of your debt to reduce your risk or to reduce the borrow fee you pay on the capital you borrow.
* **Add collateral:** The easiest way to to improve your Health Factor if your Health Factor is getting close to liquidations level, which is < 1.
* **Close Credit Account:** Closes your margin position

***

While these are about the tabs for a credit account, there are certain parameters and values you need to take care of too. They are listed below.

### Account Parameters

At the top, you can see the balance of your Credit Account denominated in the underlying asset you opened your account in (it uses ChainLink oracle prices to calculate these values).

* **Health Factor** - Your Credit Account can be liquidated if it falls below 1
* **Liquidation Price -** The price level at which your position will be liquidated
* **Quota Fee -** The fee you pay to deploy a position
* **Account Value** - Current value of Credit Account, denominated in the underlying asset;
* **Debt** - total value of the underlying asset you have borrowed from the protocol;
* **Your assets** - total value in the underlying asset that is your collateral;
* **Analytics** - check the stats of the pool and other charts in Gearbox-native analytics;
* **Etherscan** - see your Credit Account's address, and the transactions on-chain.
* **Tokens** - the list of allowed tokens as per the policy which you can trade among.

{% hint style="info" %}
Did you find a bug with the interface, something didn't work as you think it should have, or you have a suggestion on how to improve the user experience? [Suggest](https://discord.gg/hF3QvX2vgt) on Discord!
{% endhint %}
