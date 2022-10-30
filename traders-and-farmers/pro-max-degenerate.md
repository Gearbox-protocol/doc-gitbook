---
description: Some tips for absolutely degenarate farmers and traders.
---

# PRO: Max Degenerate

{% hint style="danger" %}
These tips are for traders & farmers who are absolutely degenerate. Maximum leverage, maximum risk. Exercise with caution. It's better if you are able to understand Etherscan WRITE functions in case anything goes wrong with the interface. Be careful!
{% endhint %}

### How to reach max leverage?

The protocol works without any trust or off-chain mechanisms, so the values are derived from on-chain. Even if the interface sometimes can show that your maximum leverage is reached - in reality, by interacting with the contracts on-chain, you could squeeze to the last bits!

There is the [#credit-account-min-max-borrow-limits](how-to-open-account.md#credit-account-min-max-borrow-limits "mention") which can sometimes change. But let's imagine you are in-between and don't care of the absolute values.

* Min leverage is only defined by the minimum borrow amount. It can be an x2 position if you do it with $100,000 as collateral \[your collateral worth $100K where $100,000K is the minimum limit x2 leverage = $200,000] - or can be an x1.01 if your collateral amount is $10M.

First of all, you need to understand how [Health Factor](../overview/liquidations/#what-is-a-health-factor) works. In a nutshell, all of the assets on your Credit Account are denominated in the debt asset you took as a borrowable asset. In other words, all the assets on your Credit Account in total act as collateral. Whether you have some ERC20s on your CA or farming positions - all of them have LTVs with respect to the debt asset you have chosen. [See all of the LTVs on this page](../overview/credit-account/allowedlist-policy.md#allowed-assets-list). For the calculations below, convert them from %.

{% hint style="info" %}
In case you want simple liquidation levels understanding, you can isolate positions per different debt assets. Like: stablecoin farm vs stablecoin debt asset. Or ETH Lido farms with wstETH or WETH debt. Then it's much simpler for you to know he liquidation prices. In case you cross-margin a few positions with different assets within a single Credit Account, it becomes harder. But maybe that's your goal after all, like those trying to do delta-neutral or get _paying_ longs [long.md](strategies/long.md "mention").
{% endhint %}

The math for max leverage works as follows:

$$
1 / (1 – LT)
$$

Let's say you go into Convex GUSD3crv farm \[stkcvxgusd3CRV] with debt as USDC. LTV for that is 90 so the max leverage would be: 1/(1-0,90) = 10x. That's technically the max leverage you can take which will make your HF = 1. If the deviations in assets within a farm \[assets on your Credit Account acting as collateral] never occur - then you cam remain as is.

Let's do yvCurve-stETH \[Yearn farm for stETH/ETH Curve pool] with WETH as debt. The LTV for either is 90 right now. That means 1/(1-0,90) = 10x as well.

{% hint style="info" %}
LTVs of total assets within CA <> debt assets are what determines the max.
{% endhint %}

### How to max out but more safely?

Great question, degen! You probably want to leave a bit of a leeway for some price fluctuations... Hold on, where do the prices come from? As a simple reply: currently, only Chainlink data price feeds. So this is where you should look for the source of truth, it's open to everyone on-chain.

With farming positions it's a bit more tricky.&#x20;

*







When exercising max leverage - you should keep in mind that even a few-minutes of interface not responding properly \[Infura/Alchemy downtime, bugs, whatever it is] can lead to liquidations. Everyone remembers the "oops maintaince mode" of BitMex? Well, in DeFi you can influence these cases, because the contracts are on-chain / verified - as such, you can interact with them directly without any interface. You can do so via Etherscan, your terminal, or however else.&#x20;

See the [registry of contracts](https://dev.gearbox.fi/docs/documentation/deployments/deployed-contracts/) and understand how they work to be safer!
