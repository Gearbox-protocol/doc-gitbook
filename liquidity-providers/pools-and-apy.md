---
description: 'Passive liquidity providing on Gearbox Protocol: supply & earn APY.'
---

# Pools & APY

Earning with Gearbox is as simple as lending on Compound or Aave. Next to that, the pools are isolated. Supply liquidity in the asset you choose and start earning APY!&#x20;

Your assets never end up in custody of any one person or company.

The asset you supply to the protocol would be able to be utilized, aka borrowed for leverage, by traders & farmers who would be actively rebalancing their positions or using some other strategies within the [allowed list](../overview/credit-account/#allowed-list-policy) which a [Credit Account](../overview/credit-account/) allows. As borrowers, they will be required by the protocol to pay interest rates which accrues to the underlying pools of those assets.&#x20;

![](<../.gitbook/assets/Screenshot 2021-08-07 at 22.49.25.png>)

The positions which traders and farmers take should be liquidated by third-party [liquidators](../overview/liquidations/) before the assets of liquidity providers would start being exposed to the downside. As such, the protocol returns the liquidity providers’ assets to the pools. This is how Gearbox is able to provide composable leverage.

{% hint style="warning" %}
Keep in mind that earning on Gearbox entails certain [risks](../risk-and-security/risks-terms.md), especially related to third party liquidators doing their job right. The risks presented are also general across DeFi.&#x20;
{% endhint %}

## What is a Diesel Token?

When you supply capital to a pool, you get Diesel Tokens, also known as dTokens, back. These tokens automatically earn interest & fees proportional to your share of the pool [like cTokens on Compound](https://compound.finance/docs/ctokens) or Yearn LP tokens. You don’t need to claim interest or perform any other actions, your Diesel Tokens value is supposed to grow with the protocol. _This is if the pool doesn't suffer losses from incorrect liquidations._

Getting Diesel tokens is super easy, you can try it out by [supplying liquidity to Gearbox Protocol](manage-liquidity.md#supplying-liquidity).

{% content-ref url="manage-liquidity.md" %}
[manage-liquidity.md](manage-liquidity.md)
{% endcontent-ref %}

| Asset                                                                             | Contract Address                                                                                                      |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| ETH ([WETH](../overview/faq.md#why-cant-i-trade-eth-on-dexes-via-wallet-connect)) | [0xB03670c20F87f2169A7c4eBE35746007e9575901](https://etherscan.io/address/0xB03670c20F87f2169A7c4eBE35746007e9575901) |
| WBTC                                                                              | [0xB2A015c71c17bCAC6af36645DEad8c572bA08A08](https://etherscan.io/address/0xB2A015c71c17bCAC6af36645DEad8c572bA08A08) |
| USDC                                                                              | [0x86130bDD69143D8a4E5fc50bf4323D48049E98E4](https://etherscan.io/address/0x86130bDD69143D8a4E5fc50bf4323D48049E98E4) |
| DAI                                                                               | [0x24946bCbBd028D5ABb62ad9B635EB1b1a67AF668](https://etherscan.io/address/0x24946bCbBd028D5ABb62ad9B635EB1b1a67AF668) |

## How to calculate APY?

Capital is required for traders and farmers to get leverage for their financial operations. For this, there are Liquidity Pools: anyone can become a liquidity provider by supplying assets in the Liquidity Pool. The profitability of LPs depends on the pool utilization ratio _U_ - the higher utilization, the higher interest rate.&#x20;

Borrow APY is calculated according to formula

$$
r(t) = 
    \begin{cases}
        r_0 + \frac{U(t)}{U_*}\left(r_1-r_0\right), & U(t) \le U_*\\
        r_1 + \left(U(t)-U_*\right)\frac{r_2-r_1}{1-U_*}, & U(t) > U_*.\\
    \end{cases}
$$

This model is similar to how Aave works, you can find more details in the [tech paper](../overview/whitepaper.md).

| Asset pool | r\_0 | r\_1 | r\_2 | U\_\* |
| ---------- | ---- | ---- | ---- | ----- |
| ETH        | 0    | 4    | 60   | 70    |
| WBTC       | 0    | 4    | 60   | 70    |
| USDC       | 0    | 5    | 100  | 70    |
| DAI        | 0    | 5    | 100  | 70    |

### Current Pool Caps as per latest GIP voting

| Asset | Pool max  | Min collateral | Max pers borrow |
| ----- | --------- | -------------- | --------------- |
| WETH  | 2400 WETH | 0.3WETH        | 125 WETH        |
| WBTC  | 100 WBTC  | 0.02 WBTC      | 10 WBTC         |
| USDC  | 12M USDC  | 1,000 USDC     | 500,000 USDC    |
| DAI   | 12M DAI   | 1,000 DAI      | 500,000 DAI     |

**Update #1, 18.04.2022**: governance voting for increasing limits are [here](https://snapshot.org/#/gearbox.eth/proposal/0x88f4662687cad00cfdd515fc21289a537cbe69f80ddf790a13a58bb94af3f9f1).

{% hint style="success" %}
This was established by the DAO (token holders) and multisig as [part of the first GIPs](https://gov.gearbox.fi/t/gip-1-proposal-to-add-pools/347).
{% endhint %}
