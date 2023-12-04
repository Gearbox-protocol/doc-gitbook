---
description: Previous versions since launch of V1 in 2021, to V2 in 2022, to V2.1 in 2023.
---

# OLD: V1 and V2

{% hint style="info" %}
Gearbox architecture is very modular, so it's not just that there is an allowed asset for the entire protocol - there are [different pools](../../../lending-market/pools-and-apy/) and **can even be multiple pools for the same asset**. There can be **different Credit Managers with different Allowed List policies**, etc. The information below is just an easy-to-grasp understanding for product users. Developers should dive into the tech section in [Gearbox Dev](https://dev.gearbox.fi/) docs and understand the intricacies.&#x20;

Namely, the tree goes as follows:

* Pool
  * Credit Manager
    * allowed assets
    * allowed contracts
* Credit Accounts
{% endhint %}

If you want to check and see the list of currently and old deployed contracts, go here:

{% embed url="https://dev.gearbox.fi/" %}

## Gearbox V2.1 December 2023&#x20;

### Allowed Contracts List

* sUSD and its related assets (Convex) have been disabled;
* GUSD and its related assets (Convex) have been disabled.

<table><thead><tr><th width="297">Pool</th><th>LP Token Address</th></tr></thead><tbody><tr><td>Curve ETH+stETH</td><td><a href="https://etherscan.io/address/0x06325440D014e39736583c165C2963BA99fAf14E">0x06325440D014e39736583c165C2963BA99fAf14E</a></td></tr><tr><td>Convex Curve ETH+stETH</td><td><a href="https://etherscan.io/address/0x9518c9063eB0262D791f38d8d6Eb0aca33c63ed0">0x9518c9063eB0262D791f38d8d6Eb0aca33c63ed0</a></td></tr><tr><td>Curve FRAX+3Crv</td><td><a href="https://etherscan.io/address/0xd632f22692FaC7611d2AA1C0D552930D43CAEd3B">0xd632f22692FaC7611d2AA1C0D552930D43CAEd3B</a></td></tr><tr><td>Convex Curve FRAX+3Crv</td><td><a href="https://etherscan.io/address/0xbE0F6478E0E4894CFb14f32855603A083A57c7dA">0xbE0F6478E0E4894CFb14f32855603A083A57c7dA</a></td></tr><tr><td>Curve 3pool (DAI+USDC+USDT)</td><td><a href="https://etherscan.io/address/0x6c3F90f043a72FA612cbac8115EE7e52BDe6E490">0x6c3F90f043a72FA612cbac8115EE7e52BDe6E490</a></td></tr><tr><td>Convex 3pool (DAI+USDC+USDT)</td><td><a href="https://etherscan.io/address/0x30D9410ED1D5DA1F6C8391af5338C93ab8d4035C">0x30D9410ED1D5DA1F6C8391af5338C93ab8d4035C</a></td></tr><tr><td>Curve LUSD+3Crv</td><td><a href="https://etherscan.io/address/0xEd279fDD11cA84bEef15AF5D39BB4d4bEE23F0cA">0xEd279fDD11cA84bEef15AF5D39BB4d4bEE23F0cA</a></td></tr><tr><td>Convex Curve LUSD+3Crv</td><td><a href="https://etherscan.io/address/0xFB9B2f06FDb404Fd3E2278E9A9edc8f252F273d0">0xFB9B2f06FDb404Fd3E2278E9A9edc8f252F273d0</a></td></tr><tr><td>Curve DAI+USDC+USDT+sUSD</td><td><a href="https://etherscan.io/address/0xC25a3A3b969415c80451098fa907EC722572917F">0xC25a3A3b969415c80451098fa907EC722572917F</a></td></tr><tr><td>Convex Curve DAI+USDC+USDT+sUSD</td><td><a href="https://etherscan.io/address/0x11D200ef1409cecA8D6d23e6496550f707772F11">0x11D200ef1409cecA8D6d23e6496550f707772F11</a></td></tr><tr><td>Curve GUSD+3Crv</td><td><a href="https://etherscan.io/address/0xD2967f45c4f384DEEa880F807Be904762a3DeA07">0xD2967f45c4f384DEEa880F807Be904762a3DeA07</a></td></tr><tr><td>Convex Curve GUSD+3Crv</td><td><a href="https://etherscan.io/address/0x15c2471ef46Fa721990730cfa526BcFb45574576">0x15c2471ef46Fa721990730cfa526BcFb45574576</a></td></tr><tr><td>USDC yVault</td><td><a href="https://etherscan.io/address/0xa354F35829Ae975e850e23e9615b11Da1B3dC4DE">0xa354F35829Ae975e850e23e9615b11Da1B3dC4DE</a></td></tr><tr><td>DAI yVault</td><td><a href="https://etherscan.io/address/0xdA816459F1AB5631232FE5e97a05BBBb94970c95">0xdA816459F1AB5631232FE5e97a05BBBb94970c95</a></td></tr><tr><td>WETH yVault</td><td><a href="https://etherscan.io/address/0xa258C4606Ca8206D8aA700cE2143D7db854D168c">0xa258C4606Ca8206D8aA700cE2143D7db854D168c</a></td></tr><tr><td>WBTC yVault</td><td><a href="https://etherscan.io/address/0xA696a63cc78DfFa1a63E9E50587C197387FF6C7E">0xA696a63cc78DfFa1a63E9E50587C197387FF6C7E</a></td></tr><tr><td>Curve stETH Pool yVault</td><td><a href="https://etherscan.io/address/0xdCD90C7f6324cfa40d7169ef80b12031770B4325">0xdCD90C7f6324cfa40d7169ef80b12031770B4325</a></td></tr><tr><td>Curve FRAX Pool yVault</td><td><a href="https://etherscan.io/address/0xB4AdA607B9d6b2c9Ee07A275e9616B84AC560139">0xB4AdA607B9d6b2c9Ee07A275e9616B84AC560139</a></td></tr></tbody></table>

### Allowed Assets List

* sUSD and its related assets (Convex) have been disabled;
* GUSD and its related assets (Convex) have been disabled.

<table><thead><tr><th width="210">Token</th><th width="91">USDC</th><th width="82">DAI</th><th width="90">WETH</th><th width="90">wstETH</th><th width="85">WBTC</th><th>FRAX</th></tr></thead><tbody><tr><td>WETH</td><td>85</td><td>85</td><td>94.5</td><td>90</td><td>85</td><td>85</td></tr><tr><td>stETH</td><td>82.5</td><td>82.5</td><td>90</td><td>94.5</td><td>82.5</td><td>82.5</td></tr><tr><td>WBTC</td><td>85</td><td>85</td><td>85</td><td>85</td><td>94.5</td><td>85</td></tr><tr><td>USDC</td><td>94.5</td><td>92</td><td>82.5</td><td>82.5</td><td>82.5</td><td>92</td></tr><tr><td>DAI</td><td>92</td><td>94.5</td><td>82.5</td><td>82.5</td><td>82.5</td><td>92</td></tr><tr><td>USDT</td><td>90</td><td>90</td><td>82.5</td><td>82.5</td><td>82.5</td><td>94.5</td></tr><tr><td>sUSD</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td></tr><tr><td>FRAX</td><td>90</td><td>90</td><td>82.5</td><td>82.5</td><td>82.5</td><td>90</td></tr><tr><td>gUSD</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td></tr><tr><td>LUSD</td><td>90</td><td>90</td><td>82.5</td><td>82.5</td><td>82.5</td><td>90</td></tr><tr><td>steCRV</td><td>82.5</td><td>82.5</td><td>90</td><td>90</td><td>82.5</td><td>82.5</td></tr><tr><td>cvxsteCRV</td><td>82.5</td><td>82.5</td><td>90</td><td>90</td><td>82.5</td><td>82.5</td></tr><tr><td>stkcvxsteCRV</td><td>82.5</td><td>82.5</td><td>90</td><td>90</td><td>82.5</td><td>90</td></tr><tr><td>FRAX3CRV-f</td><td>90</td><td>90</td><td>80</td><td>80</td><td>80</td><td>90</td></tr><tr><td>cvxFRAX3CRV-f</td><td>90</td><td>90</td><td>80</td><td>80</td><td>80</td><td>90</td></tr><tr><td>stkcvxFRAX3CRV</td><td>90</td><td>90</td><td>80</td><td>80</td><td>80</td><td>90</td></tr><tr><td>3Crv</td><td>90</td><td>90</td><td>80</td><td>80</td><td>80</td><td>90</td></tr><tr><td>cvx3Crv</td><td>90</td><td>90</td><td>80</td><td>80</td><td>80</td><td>90</td></tr><tr><td>stkcvx3Crv</td><td>90</td><td>90</td><td>80</td><td>80</td><td>80</td><td>90</td></tr><tr><td>LUSD3CRV-f</td><td>90</td><td>90</td><td>80</td><td>80</td><td>80</td><td>90</td></tr><tr><td>cvxLUSD3CRV-f</td><td>90</td><td>90</td><td>80</td><td>80</td><td>80</td><td>90</td></tr><tr><td>stkcvxLUSD3CRV</td><td>90</td><td>90</td><td>80</td><td>80</td><td>80</td><td>90</td></tr><tr><td>crvPlain3andSUSD</td><td>90</td><td>90</td><td>80</td><td>80</td><td>80</td><td>90</td></tr><tr><td>cvxcrvPlain3andSUSD</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td></tr><tr><td>stkcvxcrvPlain3andSUSD</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td></tr><tr><td>gusd3CRV</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td></tr><tr><td>cvxgusd3CRV</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td></tr><tr><td>stkcvxgusd3CRV</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td></tr><tr><td>FraxUsdc</td><td>90</td><td>90</td><td>80</td><td>80</td><td>80</td><td>90</td></tr><tr><td>yvDAI</td><td>90</td><td>90</td><td>80</td><td>80</td><td>80</td><td>90</td></tr><tr><td>yvUSDC</td><td>90</td><td>90</td><td>80</td><td>80</td><td>80</td><td>90</td></tr><tr><td>yvWETH</td><td>82.5</td><td>82.5</td><td>90</td><td>90</td><td>80</td><td>82.5</td></tr><tr><td>yvWBTC</td><td>82.5</td><td>82.5</td><td>80</td><td>80</td><td>90</td><td>82.5</td></tr><tr><td>yvCurve-stETH</td><td>82.5</td><td>82.5</td><td>90</td><td>90</td><td>82.5</td><td>82.5</td></tr><tr><td>yvCurve-FRAX</td><td>90</td><td>90</td><td>80</td><td>80</td><td>80</td><td>90</td></tr><tr><td>CVX</td><td>25</td><td>25</td><td>25</td><td>25</td><td>25</td><td>25</td></tr><tr><td>FXS</td><td>25</td><td>25</td><td>25</td><td>25</td><td>25</td><td>25</td></tr><tr><td>LQTY</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr><tr><td>CRV</td><td>25</td><td>25</td><td>25</td><td>25</td><td>25</td><td>25</td></tr><tr><td>LDO</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr><tr><td>SNX</td><td>25</td><td>25</td><td>25</td><td>25</td><td>25</td><td>25</td></tr></tbody></table>

***

## History: older versions in words

### Gearbox V2.1: September 2023

Gearbox V2.1 was released in June'23, the update was largely focused on improving the security of the codebase. With DeFi exploits on the rise, it was crucial to upgrade and fortify the security of the codebase. Moreover, with V3 being&#x20;

built over the existing codebase, it enabled the DAO to battle test the V3 codebase even before it's deployment. It improved security 4 ways:

* Removed access mechanisms for adapters that had lower utility
* Introduced bad debt prevention parameters
* Identified and fixed possible existing bugs&#x20;
* Improved Account security at UI and operational level

You can read the complete details in the articles below:

* [https://link.medium.com/QQOUYIVfcFb](https://link.medium.com/QQOUYIVfcFb)
* [https://link.medium.com/qdcKyjUfcFb](https://link.medium.com/qdcKyjUfcFb)

### Gearbox V2: November 2022

Gearbox V2 upgrade took place in October'22 and led to a $120M+ TVL increase. Post V1s usage, it became abundantly clear that the users are more interested in using Gearbox for Leveraged Farming than trading. V2 was thus born out of the effort to increase the avenues to leverage farm and provide a better user experience to the leverage farmers. With V2, the DAO expanded it's integrations with:

* Curve Pools
* Convex Pools
* Yearn Vaults&#x20;
* Lido Staking

This led to 14 more strategies becoming available to the users to leverage farm on. At the same time though, V1 required users to hop through multiple protocols to deploy a position. V2 was built with UX and ease of use in mind. This was brought on by:

1. **Multicall:** Multicall enabled users to open CA, perform required swaps, deploy in farm and receive LP tokens in a single transaction. While the farming happened natively on the integrated protocol, the need to leave Gearbox UI or click multiple buttons was removed.&#x20;
2. **Up to 10x Leverage:** V1 offered leverage up to 4x, this was upgraded by V2 with pools being able to offer as much as 10x leverage. This increased the max APYs a pool could produce significantly.&#x20;

The 2 factors together enabled V2 to bring leveraged farming to life. You can read more about it in the article below. You can also browse around Medium to find more info on the older V2.

{% embed url="https://medium.com/gearbox-protocol/product-evolution-v2-gearbox-protocol-from-1-to-2-going-further-dcedf3b5d959" %}

### Gearbox V1: December 2021

{% hint style="info" %}
The information about V1 Credit Managers \[Allowed List of contracts & assets] was scraped out from the docs to not confuse new users. Those CMs are still on-chain and exist, but only with the option to trade out of CA positions and close, not borrow or open new ones. If you are looking for old numbers, [check on forum](https://gov.gearbox.fi/t/pre-gip-2-3-start-gearbox-allowed-tokens-and-protocols/152/37).
{% endhint %}
