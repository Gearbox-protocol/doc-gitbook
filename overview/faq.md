---
description: Quick answers-links to the most frequently asked questions.
---

# FAQ

This section can help you find answers to the most quick questions. The other answers you can likely find by reading the page names of the docs on the left, each section explaining the topics.

* What assets and protocols are currently available? - [here](https://docs.gearbox.finance/overview/credit-account/allowedlist-policy).
* How to add new collateral / protocol? What is the framework? - [here](https://docs.gearbox.finance/overview/credit-account/how-to-add-new-assets-protocols).
* GEAR token contract and vestings? - [here](https://docs.gearbox.finance/gear-token/gear-overview).
* Funding rounds and initial supporters? - at the bottom of the page [here](https://gearboxprotocol.notion.site/Gearbox-DAO-23966f122ae4421492819242b30a0e7a).
* Current and previous DAO contributors? -at the bottom of the page [here](https://gearboxprotocol.notion.site/Gearbox-DAO-23966f122ae4421492819242b30a0e7a).
* How does the DAO work and how to join the initiatives? - [here](https://gearboxprotocol.notion.site/DAO-Initiatives-Cycles-57dea693c7f44c3d9d4d818e5b0ac88b).
* How much capital does the treasury have and where it goes? - [here](https://gearboxprotocol.notion.site/Monthly-Reports-6849871a9bae44dfb903531c0a997e8f).

{% hint style="info" %}
Do you feel like some question is missing? [Send it on Discord](https://discord.com/invite/gearbox)!
{% endhint %}

#### **- What fees am I paying to the protocol and others?**&#x20;

Since Gearbox Protocol has two sides to it, the fees you are paying depend on what user type you are. **If you are a passive Liquidity Provider, there is no direct fee for becoming one**.

If you are a leverage user, you are paying a borrow interest fee (which fluctuates depending on [utilization ratio](../lending-market/pools-and-apy.md#how-to-calculate-apy) similar to Aave) + [liquidation fees to the protocol and a liquidator](protocol-fees.md#trader-farmer-fees). The latter you pay only if you are liquidated. All these fees are configurable by [DAO](../governance/setup/). See in [protocol-fees.md](protocol-fees.md "mention").

#### - What are dTokens like dUSDC and dWBTC?&#x20;

Diesel Tokens are like cTokens of Compound. These tokens automatically earn interest & fees proportional to your share of the pool [like cTokens on Compound](https://compound.finance/docs/ctokens) or Yearn LP tokens. You don’t need to claim interest or perform any other actions, your Diesel Tokens value is supposed to grow.

#### - Will my APY for supplying liquidity go down or up?&#x20;

The APY is variable and depends on the [utilization ratio](../lending-market/pools-and-apy.md#how-to-calculate-apy) formula which is configurable by [DAO](../governance/setup/).

#### - What is a Health Factor and what can I do with it?&#x20;

[Health Factor](liquidations/#what-is-a-health-factor) is a numeric representation of your account's health. If your health factor drops below 1 or close to it, you might be liquidated. The higher the number is, the safer you are. Since liquidations make you incur higher fees, make sure to follow [tips on how to not get liquidated](../traders-and-farmers/credit-account-dashboard-overview/kak-ne-byt-rekt.md).

#### - Сan I always withdraw liquidity?

Depending on the [utilization ratio](../lending-market/pools-and-apy.md#how-to-calculate-apy) of pools, if it is high - not all the liquidity can be withdrawn at once. It doesn't mean that the protocol lost money or is insolvent - it's just that the liquidity is utilized in Credit Accounts. In such cases where available liquidity is low (which you can check in the app analytics page per pool) - the APY goes higher as to attract more capital providers and attempt to find an equilibrium. This is more or less standard among all lending-type protocols and has happened both in Compound & Aave before. _Gearbox DAO can adjust the utilization curve parameters to force certain behavior of the protocol in case weird situations occur._

See more in [#withdrawing-liquidity](../lending-market/manage-liquidity.md#withdrawing-liquidity "mention").

#### - **Why can't I borrow more?**

As the protocol has max leverage and max personal borrow parameters, which are configurable by DAO, there is a limited amount you can borrow for leverage. As such, borrowing above that amount is technically not possible. Once a Credit Account is open, you can add more collateral to increase your position size and Health Factor, but you can't borrow to infinity for security purposes.

Those shall be updated every now and then after voting, in [credit-account](credit-account/ "mention").

#### - **Why is mobile not accessible yet?**

As the protocol has gone live just recently - nobody knows what PMF (product-market fit) Gearbox has. The app will likely take many iterations, and anybody can build their own. So while this search for users and market fit are ongoing, the effort on optimiizing 100 versions at once is minimized. Later on, as things become more clear - the mobile version will be optimized and turned on.

#### - **Will Gearbox Protocol be on other chains/L2/rollups/EVM-compatible?**

Gearbox Protocol is DAO-operated, so it should be a joint community decision. That's one. If users need Gearbox - it's fine to deploy anywhere, because user-first approach.&#x20;

But it's not practical being on chains where there are not many other protocols to tap into. You see, Gearbox sources liquidity from other DeFi protocols: [trading on Uniswap and Curve, farming in Yearn](integrations.md) & etc. If a chain only has a Uniswap (original or fork) and a Curve (original or fork) it is \[1] less safe usually \[2] what is more important - it makes the product of Gearbox be inferior. If there is not much liquidity or you can't build composable positions, there isn't much to do on that chain.

So in the future there is no worry with it, but current ecosystems need to develop more and have more safe and liquid protocols to justify time and development costs. Which is likely possible, and is something to altogether discuss in 2022. See some ideas at the bottom of [this article](https://medium.com/gearbox-protocol/wen-v2-next-steps-leading-up-to-e80ec39eefe4).

#### - **Why can't I trade ETH on DEXes via Wallet Connect? Only WETH?**

Because ETH is not an ERC20 token by itself, so you can't _operate_ it like an ERC20 token which is a must-have for Gearbox Protocol and safe operations. Within the Credit Account, ETH is converted to WETH. So if you [connect via Wallet Connect](../traders-and-farmers/credit-account-dashboard-overview/connect-wallet-connect.md) or see your Credit Account on Etherscan - and check for ETH, you will see WETH only. After liquidation or closing your account, it is converted back to ETH, so liquidity providers don't need to think through this too much.

#### - Why does a trade even from stable to stable decrease my HF (health factor)?

Due to how [Threshold Weighted Values](liquidations/#threshold-weighted-value) are calculated taking into account a possible price drop and a price feed tick, a stablecoin is not actually a stablecoin for the protocol contracts. They are not 1:1. Stablecoins tend to de-peg, which must be taken into account. This keeps the protocol more secure, but also causes _max leverage_ parameter to be lower. As such, this is up to the risk appetite of Gearbox [DAO](../governance/setup/) to decide on such things.&#x20;

See the LTVs per asset-debt in [allowedlist-policy.md](credit-account/allowedlist-policy.md "mention").
