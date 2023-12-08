---
description: A quick guide to your first Credit Account.
---

# How to open a Credit Account



{% hint style="info" %}
**NOTE:** At the moment, Credit Accounts are in "Leverage Ninja" Mode as we initially test in prod: a list of addresses having access to V2 leverage. You can post your address on the [**gov forum**](https://gov.gearbox.fi/t/gip-21-leverage-ninja-mode-limits-for-v2/1572/11) with a few links. If you don't want your twitter and address to be connected publicly, you can drop a message to any of the contributors on [**Discord**](https://discord.com/invite/gearbox)**:**&#x20;
{% endhint %}

## Two paths to opening a Credit Account

Being able to leverage trade & farm starts with opening a Credit Account. However, there are different approaches in the interface that vary based on what you are looking for:

1. "I just want to leverage farm" - then you should go to [strategies](strategies/ "mention") and simply open a leveraged farming position with multicall in one click. That page lets you ape into Curve/Convex/Lido/Yearn with a single transaction, and saves you gas costs as well! It's more applicable to farmers who don't want to have a bunch of complexities and steps, and who know what end strategies they want to sit and farm in. It creates a Credit Account for you and apes into a strategy right after, removing manual complexity from you as a user.
2. "I want to have different strategies and figure out step by step" - in this case, you might be better off following the steps by yourself: from selecting the debt asset to choosing leverage, to swapping some assets and LPing into Curve, to staking on Yearn and so on. In terms of _what_ you are doing, it's the same as option 1 above, but with more steps in-between.

{% hint style="warning" %}
Before you begin, maybe check out [pro-leverage-bible.md](pro-leverage-bible.md "mention") section to understand some of the intricacies on how max leverage works.
{% endhint %}

**Step 1.** Go to [Credit Accounts](https://app.gearbox.fi/accounts) page. Click on the asset you want to borrow. This underlying debt asset is the asset you trade against, meaning all your positions are denominated in it. Once opened, the underlying asset in that particular account can't be changed. But you can open a new Credit Account with a different debt \[borrowed] asset.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2022-10-19 at 13.27.08.png" alt=""><figcaption><p><a href="https://app.gearbox.fi/accounts">https://app.gearbox.fi/accounts</a></p></figcaption></figure>

**Step 2.** Specify the amount you want to put as collateral. This will be the notional amount from which the leverage X will be calculated. As such, 1 ETH you "deposit" as notional capital can be x6 more leverage, so a 6 ETH position total. You can also have multiple collateral assets!

<figure><img src="../.gitbook/assets/Screenshot 2022-10-19 at 13.29.11 (1).png" alt=""><figcaption></figcaption></figure>

**Step 3.** Select the leverage you want to get and click "Open X position" button. Execute the approval and opening transaction as required, and that's it.

Your Credit Account is now open!&#x20;

* You can see how much borrow fees you are paying on the amount you borrowed.
* You can top up your Credit Account or borrow more... see further sections.

## Credit Account min/max borrow limits

The limits on Credit Accounts are enforced on the contract level by minimum borrow and maximum borrow limits, as per the DAO governance process - those can change. Check the latest here:

{% content-ref url="../lending-market/pools-and-apy/" %}
[pools-and-apy](../lending-market/pools-and-apy/)
{% endcontent-ref %}

{% hint style="info" %}
Did you find a bug with the interface, something didn't work as you think it should have, or you have a suggestion on how to improve the user experience? [Suggest](https://discord.gg/hF3QvX2vgt) on Discord!
{% endhint %}

Now, time to understand the dashboard:

{% content-ref url="credit-account-dashboard-overview/" %}
[credit-account-dashboard-overview](credit-account-dashboard-overview/)
{% endcontent-ref %}
