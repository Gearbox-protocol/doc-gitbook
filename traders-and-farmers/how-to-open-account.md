---
description: A quick guide to your first Credit Account.
---

# How to open a Credit Account

Being able to leverage trade & farm starts with opening a Credit Account. Simply select an interface that fits your initial purpose (farming or trading), to simplify your user journey.

{% hint style="info" %}
Underneath, the protocol logic and contracts are the same! Different dApps simply help different user bases get to their desired positions quicker.
{% endhint %}

<figure><img src="../.gitbook/assets/gearbox dapp leverage interface.png" alt=""><figcaption><p><a href="https://app.gearbox.fi/accounts">https://app.gearbox.fi/accounts</a></p></figcaption></figure>

### 1. "I want to margin trade"&#x20;

Then you better go to the PURE interface which is supposed to look like a regular familiar leverage interface. You can select the trading pair, your leverage, slippage, and all the other important parameters. _Once you open it, you can further configure the position parameters like liquidation price and leverage factor._ The [**PURE**](margin-trading-pure.md) docs page can tell you more about what it is.

<figure><img src="../.gitbook/assets/gearbox pure margin trading (1).png" alt=""><figcaption><p><a href="https://pure.gearbox.fi/">https://pure.gearbox.fi/</a></p></figcaption></figure>

{% hint style="success" %}
If you would want to get more out of margin trading, you can later click on "Extended dApp" in the interface and configure your position further. For example, make your short or long - farm at the same time. Many of these [leverage 2.0 actions](../what-can-you-do-with-leverage-2.0.md) are possible, just dive in!
{% endhint %}

### 2. "I want to leverage farm"&#x20;

Then you can check [strategies](strategies/ "mention") and open a position in one click, thanks to _multicall_. That page lets you ape into Curve/Convex/Lido/Yearn farms with a single click, saving you gas costs!

It's more applicable to farmers who don't want to have a bunch of complexities and steps, and who know what strategies they want to sit and farm in. This interface opens a Credit Account for you and apes into a strategy right after, removing manual complexity from you as a user.

_You can then change your leverage, assets, add or remove debt, etc..._

<figure><img src="../.gitbook/assets/gearbox leverage farming multicall.png" alt=""><figcaption><p><a href="https://app.gearbox.fi/strategies/list">https://app.gearbox.fi/strategies/list</a></p></figcaption></figure>

### 3. "I am 180 IQ, I will go manual"&#x20;

In this case, you might be better off following the steps by yourself: from selecting the debt asset to choosing leverage, to swapping some assets and LPing into Curve, to staking on Yearn and so on. In terms of _what_ you are doing, it's the same assets as above, but with customized steps in-between.

For this, click the small "open Credit Account" button in the Extended dApp.

<figure><img src="../.gitbook/assets/gearbox manual credit account open.png" alt=""><figcaption><p><a href="https://app.gearbox.fi/accounts">https://app.gearbox.fi/accounts</a></p></figcaption></figure>

* Select a Credit Manager based on what assets it allows for. Research the [Integrations](../overview/credit-account/allowedlist-integrations/) page to find out what specific Credit Manager you need;
* Select your assets that you want to deposit into your Credit Account;
* Select leverage factor and slippage, and then approve transactions;
* Once open, do the farm-trade operations as you choose.

<figure><img src="../.gitbook/assets/gearbox manual credit account opening.png" alt=""><figcaption><p>You can choose to deposit multiple assets at once as collateral. Then you can change your leverage factor: the higher the leverage, the lower your Health Factor. And then you can also reduce slippage. Once you open the Credit Account, you can decide to keep some of your assets as idle collateral or swap some (or all of them) into different assets. You decide!</p></figcaption></figure>

{% hint style="info" %}
Before you begin, definitely check out [pro-leverage-bible.md](pro-leverage-bible.md "mention") section to understand some of the intricacies on how max leverage works.
{% endhint %}

***

## Credit Account min/max borrow limits

The limits on Credit Accounts are enforced on the contract level by minimum borrow and maximum borrow limits. As per the DAO governance, those can change. The dApps will help you figure this out and show you the max available leverage.

In case you want to know all the tiny details on limits and LTV, check the doc in here:

{% content-ref url="../overview/credit-account/allowedlist-integrations/" %}
[allowedlist-integrations](../overview/credit-account/allowedlist-integrations/)
{% endcontent-ref %}

{% hint style="warning" %}
Did you find a bug with the interface, something didn't work as you think it should have, or you have a suggestion on how to improve the user experience? [Suggest](https://discord.gg/hF3QvX2vgt) on Discord!
{% endhint %}
