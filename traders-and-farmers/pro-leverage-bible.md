---
description: Some tips for skilled [degenerate] farmers and traders.
---

# PRO: Leverage Bible

### A different understanding of "collateral"

DeFi users are accustomed to think of collateral as "idle asset, sits there and changes my borrowing power for better or worse". With Gearbox, it's not exactly like that. That is because the entire composition of your Credit Account, whatever you have on it - be it WBTC or a farm token - acts as collateral to your debt at the same time - denominated in the debt asset, of course.&#x20;

<figure><img src="../.gitbook/assets/Gearbox Collateral Concept.png" alt=""><figcaption></figcaption></figure>

_If you go in with ETH but then swap all your assets into a stablecoin farm - your collateral now is the ERC20 representation of that stablecoin farm. Your ETH became something else._

{% hint style="info" %}
Your starting asset(s) are usually not relevant. What is important is your debt asset - and then all of the assets on your Credit Account denominated in that debt asset.
{% endhint %}

In case you want to keep your asset as truly collateral, for example you want to keep ETH yet borrow stables and grow your borrowing power, then you need to keep it idle on Credit Account:

* Open a Credit Account with debt in stablecoin (USDC CA for example)
* Put ETH in there as collateral and NOT sell it or not ape it into a position
* Borrow more stables due to ETH borrowing power

You lose some capital efficiency since not your entire position is "working", but that might be indeed your strategy. ETH goes up and u can borrow even more stables - that could work!

{% content-ref url="strategies/" %}
[strategies](strategies/)
{% endcontent-ref %}

### What is the minimum / maximum leverage?

The protocol works without any trust or off-chain mechanisms, so the values are derived from on-chain. Even if the interface sometimes can show that your maximum leverage is reached - in reality, by interacting with the contracts on-chain, you could squeeze to the last bits!

* Min leverage is only defined by the minimum borrow amount. If $100K is the min: it can be an x2 position if you do it with $100K initial capital \[your capital worth $100K where $100K is the minimum limit x2 leverage = $200K total]; or can be an x6 if your initial capital is $20K \[your capital is worth $20K and at x6 it means your position will be $120K total, so $100K borrowed].
* Now, the maximum leverage is more complex than that...

### How to calculate max leverage?

First of all, you need to understand how [Health Factor](../overview/liquidations/#what-is-a-health-factor) works. In a nutshell, all of the assets on your Credit Account are denominated in the debt asset you took as a borrowable asset. In other words, all the assets on your Credit Account in total act as collateral. Whether you have some ERC20s on your CA or farming positions - all of them have LTVs with respect to the debt asset you have chosen.

{% hint style="info" %}
In case you want simple liquidation levels, you can isolate positions per different debt assets. Like: stablecoin farm vs stablecoin debt asset. Or ETH Lido farms with wstETH or WETH as debt. Then it's much simpler for you to know the liquidation prices. In case you cross-margin a few positions with different assets within a single Credit Account, it becomes harder. But maybe that's your goal after all, like those trying to go delta-neutral or get _paying_ longs [long.md](strategies/long.md "mention").
{% endhint %}

The math for max leverage works as follows:

$$
1 / (1 – LT)
$$

Let's say you go into Convex GUSD3crv farm \[stkcvxgusd3CRV] with debt as USDC. If LTV for that is 90, the max leverage would be: 1/(1-0,90) = 10x. Let's do yvCurve-stETH \[Yearn farm for stETH/ETH Curve pool] with WETH as debt. The LTV for either is 90 right now. That means 1/(1-0,90) = 10x as well. _If LTVs for some farms become higher, more leverage could be applied._

That's technically the max leverage you can take which will make your HF = 1. If the deviations in assets within a farm \[assets on your Credit Account acting as collateral] never occur - then you can remain as is, but that's VERY risky. It's better to count in some fluctuations.

{% hint style="success" %}
You don't have to assume the worst case scenario right away. You can simply rebalance and reduce leverage \[or debt] to [avoid liquidations](credit-account-dashboard-overview/kak-ne-byt-rekt.md). If you are active in DeFi, you can take changes after sensing a farm could be worsening. No requirement to do it from the start.
{% endhint %}

### How to max out... but kinda "safely"?

These tips are for traders & farmers who are absolutely degenerate. Maximum leverage, maximum risk. Exercise with caution. It's better if you are able to understand Etherscan WRITE functions in case anything goes wrong with the interface. **Be careful and read the code!**

{% hint style="warning" %}
Keep in mind that in reality you could encounter slippage, fast price changes, and other scenarios - so don't try to squueze every last drop unless you are a MEV guru. It's better to be safe and reduce your desired leverage factor by at least a factor of 0.25 or 0.5 to account for those. It still keeps you maxed out but [helps avoid a liquidation](credit-account-dashboard-overview/kak-ne-byt-rekt.md).&#x20;
{% endhint %}

Let's say you want to go into FRAX3Crv. Out of all the assets inside, you might think that FRAX has some perceived risk. Maybe yes maybe no, doesn't matter for this exercise. Your debt asset is USDC, and you just wanna max out this farm. Let's say LTV is 90. The formula is:

$$
N = 1 / (1-LT*p)
$$



Where _N_ is the max leverage factor that you are trying to find, and _p_ is the price you think that FRAX price could drop to. Let's say you think that the lowest it could go to is $0.95. So then it is:

$$
6.896 = 1/(1-0,90*0,95)
$$

That means with leverage of x6.8 you are still fine even if FRAX price drops to $0.95.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2022-10-30 at 14.06.01.png" alt=""><figcaption><p>Let's look at what price [according to Chainlink oracles specifically] FRAX was has ever dropped to: that would be 0.9871. As such, if you don't expect it to ever go lower than historic, you might apply the following calculations: 1/(1-0,90*0,9871) = 8.959 leverage! You can find all these values on-chain yourself, but <a href="https://docs.google.com/spreadsheets/d/1kANaCnMsDWmxREsKKFGKf34uXMI5rZ-P66cJjuvkLOQ/edit?usp=sharing">check out [copy &#x26; edit] this GOOGLE SHEET to play with scenarios</a>. </p></figcaption></figure>

[**Here is the link to the sheet above.**](https://docs.google.com/spreadsheets/d/1kANaCnMsDWmxREsKKFGKf34uXMI5rZ-P66cJjuvkLOQ/edit?usp=sharing) Copy and play with the values, check scenarios, etc.

Let's try this exercise with Convex steCRV \[Curve stETH/ETH pool]. That would be:

$$
1/(1-0,90*0,935) = 6.3
$$

That is max leverage factor you can apply if you are afraid of stETH ever revisiting its lows compared to the debt asset (ETH). In case you think the lows could be 0.90 relative to ETH, then the max leverage would be: 1/(1-0,90\*0,90) = 5.26. Still, pretty damn capital efficient to farm with such leverage! _FYI, Gearbox Protocol currently uses USD Chainlink price feeds, so the ETH debt calculations are using an extra hoop when it comes to conversions._

{% hint style="warning" %}
Check [this article](https://medium.com/gearbox-protocol/product-evolution-v2-gearbox-protocol-from-1-to-2-going-further-dcedf3b5d959) about Yearn, Curve, & other oracles. And read code!
{% endhint %}

### Where do price feeds come from?

Great question, degen! You probably want to leave a bit of a leeway for some price fluctuations... Hold on, where do the prices come from? As a simple reply: currently, only Chainlink data price feeds. So this is where you should look for the source of truth, it's open to everyone on-chain.

With farming positions it's a bit more tricky. For the implementation of Curve pool oracles \[as such, Yearn & Convex positions for these assets respectively too], custom PriceFeeds look at _virtualprice \* Chainlink price of the cheapest asset inside the pool._ That is because in an event that any one asset inside a Curve pool goes down in price, the pool automatically trades into that asset. So while not a 100% will be traded into it immediately, for the safety of Gearbox Protocol, the worst case scenario is assumed when calculating the position value.

\-> [Contracts deployed are available here](https://dev.gearbox.fi/docs/documentation/deployments/deployed-contracts/).

{% hint style="info" %}
For the avoidance\* of Cream-like flash loan attacks, there is a min-max range applied to LP token price shares, which can be observed in the code/audits + mentioned in [here](https://medium.com/gearbox-protocol/product-evolution-v2-gearbox-protocol-from-1-to-2-going-further-dcedf3b5d959).

\*That is, unless a new attack vector is found. Security is important, [please verify](../risk-and-security/audits-bug-bounty.md).
{% endhint %}

### A few words about slippage

When swapping large amounts at once, you can encounter slippage. That is totally normal to have, like 0.1% on $1M is not unusual = $1K loss. But you have to keep in mind that you can't _socialize_ losses with the borrowed capital, so that loss is applied to your assets within the Credit Account only. _Otherwise it would be an attack vector that would let an attacker "lose" all Lender money._ What it means is that if you went x10 leverage on $100K of your capital, you will technically get a 1% loss on your capital, meaning -1% instantly. Sounds scary? Hold on!

That is not really an issue if you are leverage farming, because your larger position also makes back larger APY (per each leverage factor). **On a medium to long-term timeline (or even short-term) this is practically negligible.** It's the same as if you did not use leverage!

<figure><img src="../.gitbook/assets/gearbox few words about slippage.png" alt=""><figcaption></figcaption></figure>

It is less negligible if you are trading though. But, the same way slippage losses are not socialized - neither are your profits. You keep those all to yourself. Just don't... trade poorly, ok?!

{% hint style="success" %}
This is all standard. Just don't be surprised when you ape with size! **The interface shows the worst case scenario, in reality you might have not lost anything at all.**
{% endhint %}

### Doomer interface numbers

The above happens because the dApps \[both the [https://app.gearbox.fi/pools](https://app.gearbox.fi/pools) and [https://charts.gearbox.finance/pools](https://charts.gearbox.finance/pools)] use Chainlink oracles to calculate prices in the UI instead of spot prices, and those quite often deviate. So, **the interface presents an overly pessimistic scenario**. You can check Zapper instead for the prices and value of your Credit Account closer to reality. Just input your Credit Account address into [Zapper](https://zapper.fi/), and you can see all the positions there.

An even better way is to check on-chain virtual price of the positions you are in. So, the loss you are seeing in the dApps is just an honest max-pessimism scenario. Reality is always better!

{% hint style="success" %}
The same goes for slippage numbers in the interface when you try to trade & swap assets. In those cases, the interface shows the maximum drop in case your slippage, let's say if it is selected as 0.5%. Try putting it lower, and the number will improve.
{% endhint %}

<figure><img src="../.gitbook/assets/Screenshot 2022-11-11 at 18.44.06.png" alt=""><figcaption></figcaption></figure>

### Claim rewards before closing CA

The current logic doesn't always perfectly claim your unclaimed rewards, like from farming stables in Curve or Convex, so make sure to claim them before closing your Credit Account. These rewards would not be lost conceptually, but the next user of this particular CA might wake up with a nice present. _Unless you are playing a "take 100 bucks, or I double it and pass onto the next" - not recommended._ And the next user could be not you, so:

* first claim your rewards from Curve / Convex / etc.
* then close your Credit Account

<figure><img src="../.gitbook/assets/gearbox claim farming rewards.png" alt=""><figcaption></figcaption></figure>

Now, go, degen ->

{% content-ref url="how-to-open-account.md" %}
[how-to-open-account.md](how-to-open-account.md)
{% endcontent-ref %}

{% hint style="info" %}
When exercising max leverage - you should keep in mind that even a few-minutes of interface not responding properly \[Infura/Alchemy downtime, bugs, whatever it is] can lead to liquidations. Everyone remembers the "oops maintaince mode" of BitMex? Well, in DeFi you can influence these cases, because the contracts are on-chain / verified - as such, you can interact with them directly without any interface. [See the contracts](https://dev.gearbox.fi/docs/documentation/deployments/deployed-contracts/).
{% endhint %}
