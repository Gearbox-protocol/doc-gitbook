---
description: Some ideas on how leverage could be used across DeFi with the help of Gearbox.
---

# Strategies

Gearbox Protocol allows for multiple collateral types and interactions within a Credit Account. These collaterals can then deployed across protocols in order to turn DeFi strategies leveraged. Effectively, **every integration on Gearbox enables you to access multiple new strategies** basis the pools and vaults that are allowed.&#x20;

{% hint style="success" %}
Before you go any further, just know: [https://app.gearbox.fi/accounts/strategies/list](https://app.gearbox.fi/accounts/strategies/list) has the list of strategies that ape for you in one click! That's right: you configure your collateral asset(s), debt asset, leverage factor... and it does all of it for you in one click. So if you just wanna do some vanilla farming - this could be the recipe for you. But keep reading to learn about other hot stuff possible with composable leverage.
{% endhint %}

While a developer can run all of the complex interactions on-chain, executing these by going protocol to protocol is a tough task. The devs have worked this out though and the interface helps non-technical users to **ape into strategies with one click thanks to "One-Click Strategies"**.&#x20;

What it enables in 1 go:

* Open a Credit Account based on your preferred collateral, leverage, etc. selected;
* Swap some assets if needed to the ones needed for a specific farm you chose;
* LP, stake, etc. to end up in that destination as you have chosen.

Done! From assets X Y Z -> to taking leverage with gearbox -> to swaps into other assets -> to LP and then staking in the protocols you chose. **All in one click thanks to Multicall + Smart Router!**

<figure><img src="../../.gitbook/assets/Screenshot 2022-10-27 at 19.50.34.png" alt=""><figcaption><p><a href="https://app.gearbox.fi/accounts/strategies/list">https://app.gearbox.fi/accounts/strategies/list</a></p></figcaption></figure>

## Concrete Strategy Examples

**Leveraged Liquid Staking**: Stake ETH on LIDO to get stETH. The stETH can then further enable multiple further avenues of incremental APY. You can read the complete details below

{% content-ref url="leveraged-liquid-staking.md" %}
[leveraged-liquid-staking.md](leveraged-liquid-staking.md)
{% endcontent-ref %}

**Leveraged Stablecoin Farming:** With V2, we'll be adding a few different stablecoins to help you access more stablecoin strategies as well as gain control over what all stablecoins you have and want exposure to, you can see the exact details below:

{% content-ref url="leveraged-stablecoin-farming.md" %}
[leveraged-stablecoin-farming.md](leveraged-stablecoin-farming.md)
{% endcontent-ref %}

**Leveraged Vanilla yVaults:** This is a great way to avoid any funding fee while leveraging BTC and ETH and earning a small APY through yVaults

{% content-ref url="leveraged-vanilla-yvaults.md" %}
[leveraged-vanilla-yvaults.md](leveraged-vanilla-yvaults.md)
{% endcontent-ref %}

{% hint style="info" %}
Do you have a strategy or idea which you would like to build on top of Gearbox or find community members who could help you out get un-rekt? Jump into [Discord](https://discord.gg/dtqqwDuawE)!
{% endhint %}

Some older V1 primitive examples \[that still work though of course]:

{% content-ref url="long.md" %}
[long.md](long.md)
{% endcontent-ref %}

{% content-ref url="arb-correlated-assets.md" %}
[arb-correlated-assets.md](arb-correlated-assets.md)
{% endcontent-ref %}

