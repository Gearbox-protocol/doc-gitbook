---
description: >-
  These are the safer strategies that still encapsulate a directional trade.
  Great for avoiding funding fee or reducing the overall fee paid.
---

# Leveraged Vanilla yVaults

<figure><img src="../../.gitbook/assets/Screenshot 2022-10-26 at 9.32.54 PM.png" alt=""><figcaption></figcaption></figure>

#### ETH yVault <a href="#8304" id="8304"></a>

This is the vanilla ETH yVault by Yearn (technically it uses Wrapped ETH, but who’s keeping track).

This vault has access to a variety of strategies including lending ETH on platforms like Aave, Compound, Alpha Homora, 88MPH, and others. Other strategies include supplying ETH on Curve, Balancer for liquidity provision.

To see the full list of possible strategies, you can [check out the Yearn docs](https://vaults.yearn.finance/ethereum/defi-tokens#0xa258C4606Ca8206D8aA700cE2143D7db854D168c).

This vault is the “vanilla” ETH vault, and fairly or unfairly, is generally seen as ‘safer’ than other more exotic ETH strategies like the stETH Curve vault mentioned above. Correspondingly, the APY on this vault is somewhat lower than on the stETH vault. Potentially, the APY on the ETH yVault will tend to fluctuate based on how much demand there is to borrow ETH.

#### WBTC yVault <a href="#4f09" id="4f09"></a>

This is Yearn vault for WBTC, or wrapped BTC.

The vault uses a large variety of strategies, including lending on Aave and Compound and LPing on Curve and Balancer among a wide variety of other strategies ([see the full list of possible strategies here](https://vaults.yearn.finance/ethereum/defi-tokens#0xA696a63cc78DfFa1a63E9E50587C197387FF6C7E)).

The yield on this vault tends to be quite low as there is not all that much defi activity where use of WBTC is required, which in turn means that there is often not that much demand to borrow WBTC. Defi yields using BTC as a base asset are hard to come by.

Still, if you deposit into the WBTC yVault, when there is an opportunity to earn decent yields on WBTC, you can bet that the smart folks over at Yearn will be among the first to find it, so the WBTC yVault is a pretty good place to park your BTC if you’re a bitcoin enthusiast who wants to participate in DeFi.
