---
description: Constantly updated list of Allowed Tokens and Contracts.
---

# AllowedList: Integrations

Composability of Gearbox Protocol is possible via forever-increasing list of Allowed Tokens and Allowed Contracts. By allowing users to access more trade routes, deposits, farms, interactions - the [composability](../../../what-can-you-do-with-leverage-2.0.md) of Gearbox Protocol can really shine!&#x20;

<figure><img src="../../../.gitbook/assets/gearbox integrations.png" alt=""><figcaption></figcaption></figure>

Conceptually, Gearbox has developed integrations for: Uniswap, Sushiswap, Convex, Yearn, Curve, Balancer, Aura, and some others. However, when it comes to farming or LPing - an integration wih a protocol doesn't mean all of its assets and pools. That is because many protocols have non-generalized pools, with different price oracles required for each, and so on.

See V3 code in here to give you a glimpse:&#x20;

{% embed url="https://github.com/Gearbox-protocol/integrations-v3/" %}

Also, Gearbox architecture is modular, so it's not just that there is an Allowed Asset for the entire protocol - there are different pools and **can even be multiple pools for the same asset**. There can be **different Credit Managers with different Allowed List policies**, etc. Developers should dive into the tech section in Gearbox Dev docs and understand the intricacies. It goes like this:

* Pool
  * Credit Manager
    * allowed assets
    * allowed contracts
* Credit Accounts

{% hint style="success" %}
The AllowedList is basically a permission box, but within that box - all the actions are permissionless. You decide how to apply leverage, where to apply it, how to trade assets and when. There are no vaults or pre-made strategies here, you can manage it however you want within the Allowed List permissions. Extended dApp can be easier for complex operations. You can, of course, also manage it all fully onchain with your own infrastructure!
{% endhint %}

Please check the onchain contracts for the latest, as below might be updating with delays.

### CreditManager Trade USDC Tier 1

| Asset           | Liquidation Threshold |
| --------------- | --------------------- |
| USDC            | 94.5%                 |
| WETH            | 90%                   |
| WBTC            | 90%                   |
| STETH           | 90%                   |
| DAI             | 90%                   |
| USDT            | 90%                   |
| yvWETH          | 87%                   |
| yvWBTC          | 87%                   |
| 3Crv            | 0%                    |
| crvUSDTWBTCWETH | 0%                    |
| steCRV          | 0%                    |
| sDAI            | 90%                   |
| yvUSDC          | 90%                   |
| yvDAI           | 90%                   |

### CreditManager Trade USDC Tier 2

| Asset | Liquidation Threshold |
| ----- | --------------------- |
| USDC  | 94.5%                 |
| WETH  | 90%                   |
| DAI   | 90%                   |
| USDT  | 90%                   |
| MKR   | 82.5%                 |
| UNI   | 82.5%                 |
| LINK  | 82.5%                 |
| LDO   | 82.5%                 |

### CreditManager Trade USDC Tier 3

| Asset        | Liquidation Threshold |
| ------------ | --------------------- |
| USDC         | 94.5%                 |
| WETH         | 90%                   |
| DAI          | 90%                   |
| USDT         | 90%                   |
| FRAX         | 90%                   |
| CRV          | 72.5%                 |
| CVX          | 72.5%                 |
| FXS          | 72.5%                 |
| APE          | 72.5%                 |
| crvCVXETH    | 0%                    |
| crvUSDETHCRV | 0%                    |
| crvUSD       | 0%                    |

### CreditManager Farm USDC

| Asset                 | Liquidation Threshold |
| --------------------- | --------------------- |
| USDC                  | 94.5%                 |
| WETH                  | 90%                   |
| DAI                   | 90%                   |
| USDT                  | 90%                   |
| FRAX                  | 90%                   |
| sDAI                  | 90%                   |
| yvUSDC                | 90%                   |
| yvDAI                 | 90%                   |
| stkcvxcrvUSDUSDC      | 87%                   |
| stkcvxcrvUSDUSDT      | 87%                   |
| stkcvxcrvUSDFRAX      | 87%                   |
| stkcvxcrvFRAX         | 87%                   |
| CRV                   | 72.5%                 |
| CVX                   | 72.5%                 |
| crvUSDUSDC            | 0%                    |
| cvxcrvUSDUSDC         | 0%                    |
| crvUSDUSDT            | 0%                    |
| cvxcrvUSDUSDT         | 0%                    |
| crvUSDFRAX            | 0%                    |
| cvxcrvUSDFRAX         | 0%                    |
| crvFRAX               | 0%                    |
| cvxcrvFRAX            | 0%                    |
| 3Crv                  | 0%                    |
| crvCVXETH             | 0%                    |
| crvUSDETHCRV          | 0%                    |
| crvUSD                | 0%                    |
| # Pool Trade WBTC v3: |                       |

### CreditManager Trade WBTC Tier 1

| Asset           | Liquidation Threshold |
| --------------- | --------------------- |
| WBTC            | 94.5%                 |
| WETH            | 90%                   |
| USDC            | 90%                   |
| USDT            | 90%                   |
| STETH           | 90%                   |
| DAI             | 90%                   |
| yvWETH          | 87%                   |
| sDAI            | 87%                   |
| yvUSDC          | 87%                   |
| 3Crv            | 0%                    |
| crvUSDTWBTCWETH | 0%                    |
| steCRV          | 0%                    |
| yvWBTC          | 90%                   |

### CreditManager Trade WBTC Tier 2

| Asset           | Liquidation Threshold |
| --------------- | --------------------- |
| WBTC            | 94.5%                 |
| USDC            | 90%                   |
| WETH            | 90%                   |
| DAI             | 90%                   |
| USDT            | 90%                   |
| MKR             | 82.5%                 |
| UNI             | 82.5%                 |
| LINK            | 82.5%                 |
| LDO             | 82.5%                 |
| crvUSDTWBTCWETH | 0%                    |

### CreditManager Trade WBTC Tier 3

| Asset                 | Liquidation Threshold |
| --------------------- | --------------------- |
| WBTC                  | 94.5%                 |
| USDC                  | 90%                   |
| WETH                  | 90%                   |
| DAI                   | 90%                   |
| USDT                  | 90%                   |
| FRAX                  | 90%                   |
| CRV                   | 72.5%                 |
| CVX                   | 72.5%                 |
| FXS                   | 72.5%                 |
| APE                   | 72.5%                 |
| crvCVXETH             | 0%                    |
| crvUSDETHCRV          | 0%                    |
| crvUSD                | 0%                    |
| crvUSDTWBTCWETH       | 0%                    |
| # Pool Trade WETH v3: |                       |

### CreditManager Trade WETH Tier 1

| Asset           | Liquidation Threshold |
| --------------- | --------------------- |
| WETH            | 94.5%                 |
| USDC            | 90%                   |
| WBTC            | 90%                   |
| STETH           | 90%                   |
| DAI             | 90%                   |
| USDT            | 90%                   |
| yvUSDC          | 87%                   |
| yvWBTC          | 87%                   |
| sDAI            | 87%                   |
| 3Crv            | 0%                    |
| crvUSDTWBTCWETH | 0%                    |
| steCRV          | 0%                    |
| yvWETH          | 90%                   |

### CreditManager Trade WETH Tier 2

| Asset | Liquidation Threshold |
| ----- | --------------------- |
| WETH  | 94.5%                 |
| USDC  | 90%                   |
| DAI   | 90%                   |
| USDT  | 90%                   |
| MKR   | 82.5%                 |
| UNI   | 82.5%                 |
| LINK  | 82.5%                 |
| LDO   | 82.5%                 |

### CreditManager Trade WETH Tier 3

| Asset        | Liquidation Threshold |
| ------------ | --------------------- |
| WETH         | 94.5%                 |
| USDC         | 90%                   |
| DAI          | 90%                   |
| USDT         | 90%                   |
| FRAX         | 90%                   |
| CRV          | 72.5%                 |
| CVX          | 72.5%                 |
| FXS          | 72.5%                 |
| APE          | 72.5%                 |
| crvCVXETH    | 0%                    |
| crvUSDETHCRV | 0%                    |
| crvUSD       | 0%                    |

### CreditManager Farm WETH

| Asset                      | Liquidation Threshold |
| -------------------------- | --------------------- |
| WETH                       | 94.5%                 |
| WBTC                       | 90%                   |
| USDT                       | 90%                   |
| STETH                      | 90%                   |
| rETH                       | 90%                   |
| weETH                      | 90%                   |
| osETH                      | 90%                   |
| yvWETH                     | 90%                   |
| stkcvxcrvUSDETHCRV         | 85%                   |
| stkcvxcrvUSDTWBTCWETH      | 85%                   |
| auraB\_rETH\_STABLE\_vault | 87%                   |
| CRV                        | 72.5%                 |
| CVX                        | 72.5%                 |
| BAL                        | 0%                    |
| AURA                       | 0%                    |
| SWISE                      | 0%                    |
| crvUSDETHCRV               | 0%                    |
| cvxcrvUSDETHCRV            | 0%                    |
| crvUSDTWBTCWETH            | 0%                    |
| cvxcrvUSDTWBTCWETH         | 0%                    |
| B\_rETH\_STABLE            | 0%                    |
| auraB\_rETH\_STABLE        | 0%                    |
| steCRV                     | 0%                    |
| crvUSD                     | 0%                    |
| crvCVXETH                  | 0%                    |
| rETH\_f                    | 0%                    |

### CreditManager Restaking WETH

| Asset   | Liquidation Threshold |
| ------- | --------------------- |
| WETH    | 96%                   |
| weETH   | 91.5%                 |
| ezETH   | 91.5%                 |
| rETH    | 0%                    |
| rETH\_f | 0%                    |

If you want to check and see the list of deployed contracts, go here:

{% embed url="https://dev.gearbox.fi/" %}
