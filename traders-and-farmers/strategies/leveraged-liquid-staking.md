---
description: How leveraged liquid staking strategies can work with LIDO and others.
---

# Leveraged liquid staking

With the Gearbox integration, you are able to lever up staking as per your risk and debt \[borrowed] asset preference to get access to true leveraged staking… But that’s just the tip of the iceberg. **Beyond the leveraged ETH, it’s the stETH you receive that enables composability across multiple more DeFi protocols**. And each protocol enables you to earn even more APY. Here are the possible strategies, **all available through One Click.**

### Pure leveraged staking yields in stETH <a href="#a600" id="a600"></a>

The stETH is what you receive when you stake ETH, with the ability to deploy directly on the [LIDO protocol](https://stake.lido.fi/). stETH ideally is supposed to maintain a _peg_ against ETH but market conditions can make it lose peg which can lead to your health factor dropping, this has previously happened and you should manage your risk accordingly. Depends on your debt asset too!

{% hint style="success" %}
The yield here is the rebasing stETH rewards you receive. If they are more than the borrow rates you receive, this fully makes sense. This also makes sense if you went ETH-long relative to stablecoin debt: [long.md](long.md "mention")
{% endhint %}

<figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption><p><a href="https://app.gearbox.fi/accounts">https://app.gearbox.fi/accounts</a></p></figcaption></figure>

### Convex stETHcrv <a href="#82c4" id="82c4"></a>

Convex Finance allows users to stake steCRV LP tokens into their vault, to farm LDO, CVX, trading fees, as well as boosted CRV rewards — without the need for users to lock-up CRV themselves. This is on top of the staking APY of stETH (the portion that remains as stETH inside Curve pool).

{% hint style="success" %}
Yield: a mix of CVX, LDO, boosted CRV, staking yields, and trading fees of Curve pool.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption><p><a href="https://app.gearbox.fi/accounts">https://app.gearbox.fi/accounts</a></p></figcaption></figure>

### Yearn stETHCrv <a href="#cc9e" id="cc9e"></a>

Yearn has very similar sources of yield to Convex but unlike convex it sells off some of the rewards earned to then redeposit ETH/stETH into the vault. Without fees, usually has higher performance.

{% hint style="success" %}
Yield: a mix of CVX, LDO, boosted CRV, staking yields, and trading fees of Curve pool.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (12).png" alt=""><figcaption><p><a href="https://app.gearbox.fi/accounts">https://app.gearbox.fi/accounts</a></p></figcaption></figure>

### Curve stETH <a href="#471f" id="471f"></a>

The Curve stETH Pool takes Lido stETH (liquid staked ETH), puts it in a curve pool with vanilla ETH.

{% hint style="success" %}
Yield: a mix of LDO, CRV, staking yields, and trading fees of Curve pool.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (10).png" alt=""><figcaption><p><a href="https://app.gearbox.fi/accounts">https://app.gearbox.fi/accounts</a></p></figcaption></figure>

### cbETH

Like stETH, cbETH or Coinbase Wrapped Staked ETH is an ERC20 based liquid representation of a customer’s staked-ETH. cbETH has grown over time to become the second biggest LSD service after LIDO. The addition of the&#x20;
