---
description: Constantly updated list of Allowed Tokens and Contracts.
---

# AllowedList Policy

Composability of Gearbox Protocol is possible via forever-increasing list of Allowed Tokens and Allowed Contracts. By allowing users to access more trade routes, deposits, farms, interactions - the [composability](../../leverage-2.0-is-composable.md) of Gearbox Protocol can really shine! This page is dedicated to keeping an up-to-date list of Allowed Tokens and Allowed Contracts.

{% hint style="info" %}
Gearbox architecture is very modular, so it's not just that there is an allowed asset for the entire protocol - there are different pools and **can even be multiple pools for the same asset**. There can be **different Credit Managers with different Allowed List policies**, etc. The information below is just an easy-to-grasp understanding for product users. Developers should dive into the tech section in Gearbox Dev docs and understand the intricacies. Namely, the tree goes as follows:

* Pool
  * Credit Manager
    * allowed assets
    * allowed contracts
* Credit Accounts
{% endhint %}

If you want to check and see the list of deployed contracts, go here:

{% embed url="https://dev.gearbox.fi/" %}

{% hint style="success" %}
Decision on the assets and contracts as per [GIP-19](https://gov.gearbox.fi/t/gip-19-v2-discussion-pools-assets-and-allowedlist-policy-for-v2/1438). And further GIPs.
{% endhint %}

### Allowed Contracts List

| Pool                            | LP Token Address                                                                                                      |
| ------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| Curve ETH+stETH                 | [0x06325440D014e39736583c165C2963BA99fAf14E](https://etherscan.io/address/0x06325440D014e39736583c165C2963BA99fAf14E) |
| Convex Curve ETH+stETH          | [0x9518c9063eB0262D791f38d8d6Eb0aca33c63ed0](https://etherscan.io/address/0x9518c9063eB0262D791f38d8d6Eb0aca33c63ed0) |
| Curve FRAX+3Crv                 | [0xd632f22692FaC7611d2AA1C0D552930D43CAEd3B](https://etherscan.io/address/0xd632f22692FaC7611d2AA1C0D552930D43CAEd3B) |
| Convex Curve FRAX+3Crv          | [0xbE0F6478E0E4894CFb14f32855603A083A57c7dA](https://etherscan.io/address/0xbE0F6478E0E4894CFb14f32855603A083A57c7dA) |
| Curve 3pool (DAI+USDC+USDT)     | [0x6c3F90f043a72FA612cbac8115EE7e52BDe6E490](https://etherscan.io/address/0x6c3F90f043a72FA612cbac8115EE7e52BDe6E490) |
| Convex 3pool (DAI+USDC+USDT)    | [0x30D9410ED1D5DA1F6C8391af5338C93ab8d4035C](https://etherscan.io/address/0x30D9410ED1D5DA1F6C8391af5338C93ab8d4035C) |
| Curve LUSD+3Crv                 | [0xEd279fDD11cA84bEef15AF5D39BB4d4bEE23F0cA](https://etherscan.io/address/0xEd279fDD11cA84bEef15AF5D39BB4d4bEE23F0cA) |
| Convex Curve LUSD+3Crv          | [0xFB9B2f06FDb404Fd3E2278E9A9edc8f252F273d0](https://etherscan.io/address/0xFB9B2f06FDb404Fd3E2278E9A9edc8f252F273d0) |
| Curve DAI+USDC+USDT+sUSD        | [0xC25a3A3b969415c80451098fa907EC722572917F](https://etherscan.io/address/0xC25a3A3b969415c80451098fa907EC722572917F) |
| Convex Curve DAI+USDC+USDT+sUSD | [0x11D200ef1409cecA8D6d23e6496550f707772F11](https://etherscan.io/address/0x11D200ef1409cecA8D6d23e6496550f707772F11) |
| Curve GUSD+3Crv                 | [0xD2967f45c4f384DEEa880F807Be904762a3DeA07](https://etherscan.io/address/0xD2967f45c4f384DEEa880F807Be904762a3DeA07) |
| Convex Curve GUSD+3Crv          | [0x15c2471ef46Fa721990730cfa526BcFb45574576](https://etherscan.io/address/0x15c2471ef46Fa721990730cfa526BcFb45574576) |
| USDC yVault                     | [0xa354F35829Ae975e850e23e9615b11Da1B3dC4DE](https://etherscan.io/address/0xa354F35829Ae975e850e23e9615b11Da1B3dC4DE) |
| DAI yVault                      | [0xdA816459F1AB5631232FE5e97a05BBBb94970c95](https://etherscan.io/address/0xdA816459F1AB5631232FE5e97a05BBBb94970c95) |
| WETH yVault                     | [0xa258C4606Ca8206D8aA700cE2143D7db854D168c](https://etherscan.io/address/0xa258C4606Ca8206D8aA700cE2143D7db854D168c) |
| WBTC yVault                     | [0xA696a63cc78DfFa1a63E9E50587C197387FF6C7E](https://etherscan.io/address/0xA696a63cc78DfFa1a63E9E50587C197387FF6C7E) |
| Curve stETH Pool yVault         | [0xdCD90C7f6324cfa40d7169ef80b12031770B4325](https://etherscan.io/address/0xdCD90C7f6324cfa40d7169ef80b12031770B4325) |
| Curve FRAX Pool yVault          | [0xB4AdA607B9d6b2c9Ee07A275e9616B84AC560139](https://etherscan.io/address/0xB4AdA607B9d6b2c9Ee07A275e9616B84AC560139) |

### Allowed Assets List

Each column is the pool denomination asset, so the % LTV values per different asset are specific to each pool. As such, leverage factor on correlated assets \[stable to stable] can be higher! Links to all the ERC20 contracts can be found [here](https://gov.gearbox.fi/t/gip-19-v2-discussion-pools-assets-and-allowedlist-policy-for-v2/1438), they do not fit into gitbook table format.

{% hint style="info" %}
If working with the raw numbers, [LT](../liquidations/#liquidation-threshold) for stables would work as follows: a swap from a stablecoin to a stablecoin would cause your [Health Factor](../../traders-and-farmers/credit-account-dashboard-overview/kak-ne-byt-rekt.md#what-i-can-do-if-my-health-factor-is-close-to-1-to-keep-my-credit-account-alive) to decrease, that is because stables are not always stable from the price feed and risks perspective. It's not safe to assume a stable is 1:1 to another one, so there are more [complex calculations being done](../liquidations/#threshold-weighted-value) which account for possible slippage, chainlink price tick, and other factors.
{% endhint %}



| Token                  | USDC | DAI  | WETH | wstETH | WBTC | FRAX |
| ---------------------- | ---- | ---- | ---- | ------ | ---- | ---- |
| WETH                   | 85   | 85   | 94.5 | 90     | 85   | 85   |
| stETH                  | 82.5 | 82.5 | 90   | 94.5   | 82.5 | 82.5 |
| WBTC                   | 85   | 85   | 85   | 85     | 94.5 | 85   |
| USDC                   | 94.5 | 92   | 82.5 | 82.5   | 82.5 | 92   |
| DAI                    | 92   | 94.5 | 82.5 | 82.5   | 82.5 | 92   |
| USDT                   | 90   | 90   | 82.5 | 82.5   | 82.5 | 94.5 |
| sUSD                   | 90   | 90   | 82.5 | 82.5   | 82.5 | 90   |
| FRAX                   | 90   | 90   | 82.5 | 82.5   | 82.5 | 90   |
| gUSD                   | 90   | 90   | 82.5 | 82.5   | 82.5 | 90   |
| LUSD                   | 90   | 90   | 82.5 | 82.5   | 82.5 | 90   |
| steCRV                 | 82.5 | 82.5 | 90   | 90     | 82.5 | 82.5 |
| cvxsteCRV              | 82.5 | 82.5 | 90   | 90     | 82.5 | 82.5 |
| stkcvxsteCRV           | 82.5 | 82.5 | 90   | 90     | 82.5 | 90   |
| FRAX3CRV-f             | 90   | 90   | 80   | 80     | 80   | 90   |
| cvxFRAX3CRV-f          | 90   | 90   | 80   | 80     | 80   | 90   |
| stkcvxFRAX3CRV         | 90   | 90   | 80   | 80     | 80   | 90   |
| 3Crv                   | 90   | 90   | 80   | 80     | 80   | 90   |
| cvx3Crv                | 90   | 90   | 80   | 80     | 80   | 90   |
| stkcvx3Crv             | 90   | 90   | 80   | 80     | 80   | 90   |
| LUSD3CRV-f             | 90   | 90   | 80   | 80     | 80   | 90   |
| cvxLUSD3CRV-f          | 90   | 90   | 80   | 80     | 80   | 90   |
| stkcvxLUSD3CRV         | 90   | 90   | 80   | 80     | 80   | 90   |
| crvPlain3andSUSD       | 90   | 90   | 80   | 80     | 80   | 90   |
| cvxcrvPlain3andSUSD    | 90   | 90   | 80   | 80     | 80   | 90   |
| stkcvxcrvPlain3andSUSD | 90   | 90   | 80   | 80     | 80   | 90   |
| gusd3CRV               | 90   | 90   | 80   | 80     | 80   | 90   |
| cvxgusd3CRV            | 90   | 90   | 80   | 80     | 80   | 90   |
| stkcvxgusd3CRV         | 90   | 90   | 80   | 80     | 80   | 90   |
| FraxUsdc               | 90   | 90   | 80   | 80     | 80   | 90   |
| yvDAI                  | 90   | 90   | 80   | 80     | 80   | 90   |
| yvUSDC                 | 90   | 90   | 80   | 80     | 80   | 90   |
| yvWETH                 | 82.5 | 82.5 | 90   | 90     | 80   | 82.5 |
| yvWBTC                 | 82.5 | 82.5 | 80   | 80     | 90   | 82.5 |
| yvCurve-stETH          | 82.5 | 82.5 | 90   | 90     | 82.5 | 82.5 |
| yvCurve-FRAX           | 90   | 90   | 80   | 80     | 80   | 90   |
| CVX                    | 25   | 25   | 25   | 25     | 25   | 25   |
| FXS                    | 25   | 25   | 25   | 25     | 25   | 25   |
| LQTY                   | 0    | 0    | 0    | 0      | 0    | 0    |
| CRV                    | 25   | 25   | 25   | 25     | 25   | 25   |
| LDO                    | 0    | 0    | 0    | 0      | 0    | 0    |
| SNX                    | 25   | 25   | 25   | 25     | 25   | 25   |

{% hint style="info" %}
The information about V1 Credit Managers \[Allowed List of contracts & assets] was scraped out from the docs to not confuse new users. Those CMs are still on-chain and exist, but only with the option to trade out of CA positions and close, not borrow or open new ones. If you are looking for old numbers, [check on forum](https://gov.gearbox.fi/t/pre-gip-2-3-start-gearbox-allowed-tokens-and-protocols/152/37).
{% endhint %}
