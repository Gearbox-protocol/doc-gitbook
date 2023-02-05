---
description: 'Passive liquidity providing on Gearbox Protocol: supply & earn APY.'
---

# Pools & APY

Earning with Gearbox is as simple as lending on Compound or Aave. Next to that, the pools are isolated. Supply liquidity in the asset you choose and start earning APY!&#x20;

Your assets never end up in custody of any one person or company.

The asset you supply to the protocol would be able to be utilized, aka borrowed for leverage, by traders & farmers who would be actively rebalancing their positions or using some other strategies within the [AllowedList](../overview/credit-account/#allowed-list-policy) which a [Credit Account](../overview/credit-account/) allows. As borrowers, they will be required by the protocol to pay interest rates which accrues to the underlying pools of those assets.&#x20;

![](<../.gitbook/assets/Screenshot 2021-08-07 at 22.49.25.png>)

The positions which traders and farmers take should be liquidated by third-party [liquidators](../overview/liquidations/) before the assets of liquidity providers would start being exposed to the downside. As such, the protocol returns the liquidity providers’ assets to the pools. This is how Gearbox is able to provide composable leverage.

{% hint style="info" %}
Keep in mind that earning on Gearbox entails certain [risks](../risk-and-security/risks-terms.md), especially related to third party liquidators doing their job right. The risks presented are also general across DeFi.&#x20;
{% endhint %}

## What is a Diesel Token?

When you supply capital to a pool, you get Diesel Tokens, also known as dTokens, back. These tokens automatically earn interest & fees proportional to your share of the pool [like cTokens on Compound](https://compound.finance/docs/ctokens) or Yearn LP tokens. You don’t need to claim interest or perform any other actions, your Diesel Tokens grow in value. _This is if the pool doesn't suffer losses from incorrect liquidations._

Getting Diesel tokens is super easy, you can try it out by [supplying liquidity to Gearbox Protocol](manage-liquidity.md#supplying-liquidity).

{% content-ref url="manage-liquidity.md" %}
[manage-liquidity.md](manage-liquidity.md)
{% endcontent-ref %}

| Asset                                                                             | Contract Address                                                                                                      |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| ETH ([WETH](../overview/faq.md#why-cant-i-trade-eth-on-dexes-via-wallet-connect)) | [0xB03670c20F87f2169A7c4eBE35746007e9575901](https://etherscan.io/address/0xB03670c20F87f2169A7c4eBE35746007e9575901) |
| wstETH                                                                            | [0xB8cf3Ed326bB0E51454361Fb37E9E8df6DC5C286](https://etherscan.io/address/0xB8cf3Ed326bB0E51454361Fb37E9E8df6DC5C286) |
| USDC                                                                              | [0x86130bDD69143D8a4E5fc50bf4323D48049E98E4](https://etherscan.io/address/0x86130bDD69143D8a4E5fc50bf4323D48049E98E4) |
| DAI                                                                               | [0x24946bCbBd028D5ABb62ad9B635EB1b1a67AF668](https://etherscan.io/address/0x24946bCbBd028D5ABb62ad9B635EB1b1a67AF668) |
| WBTC                                                                              | [0xB2A015c71c17bCAC6af36645DEad8c572bA08A08](https://etherscan.io/address/0xB2A015c71c17bCAC6af36645DEad8c572bA08A08) |

## How to calculate APY?

Capital is required for traders and farmers to get leverage for their financial operations. For this, there are Liquidity Pools: anyone can become a liquidity provider by supplying assets in the Liquidity Pool. The profitability of LPs depends on the pool utilization ratio _U_ - the higher utilization, the higher interest rate. See a bit more on the [protocol-fees.md](../overview/protocol-fees.md "mention") page.

Borrow APY is calculated according to formula

$$
r(t) = 
    \begin{cases}
        r_0 + \frac{U(t)}{U_*}\left(r_1-r_0\right), & U(t) \le U_*\\
        r_1 + \left(U(t)-U_*\right)\frac{r_2-r_1}{1-U_*}, & U(t) > U_*.\\
    \end{cases}
$$

This model is similar to how Aave works.

| Asset pool | r\_0 | r\_1 | r\_2 | U\_\* |
| ---------- | ---- | ---- | ---- | ----- |
| USDC       | 0    | 1.5  | 100  | 85    |
| DAI        | 0    | 1.5  | 100  | 85    |
| wstETH     | 0    | 1    | 60   | 85    |
| ETH        | 0    | 2.5  | 60   | 85    |
| WBTC       | 0    | 2.5  | 60   | 85    |

****[**Latest update**](https://gov.gearbox.fi/t/gip-20-update-fees-interest-rate-curves/1571): governance voting to change pool interest rate curve parameters and make the curve more flat as a bootstrap mechanism for V2 Leverage Ninja launch. See the [logic](https://gov.gearbox.fi/t/gip-20-update-fees-interest-rate-curves/1571).

### Current Pool Caps as per latest GIP voting

| Asset  | Pool max | Min pers borrow | Max pers borrow |
| ------ | -------- | --------------- | --------------- |
| USDC   | N/A      | 100,000 USDC    | 1,000,000 USDC  |
| DAI    | N/A      | 100,000 DAI     | 1,000,000 DAI   |
| wstETH | N/A      | 75 wstETH       | 600 wstETH      |
| WETH   | N/A      | 75 WETH         | 600 WETH        |
| WBTC   | N/A      | 5.5 WBTC        | 50 WBTC         |

****[**Latest update**](https://gov.gearbox.fi/t/gip-20-update-fees-interest-rate-curves/1571)**:** pool limits are effectively lifted. Any actual caps are just required by the architecture to have \*some\* number and can be lifted without a vote if the TVL approaches them. As for the min-max personal borrow limits, they have been established by another vote: [GIP-21](https://gov.gearbox.fi/t/gip-21-leverage-ninja-mode-limits-for-v2/1572).
