---
description: Constantly updated list of Allowed Tokens and Contracts.
---

# AllowedList Policy

Composability of Gearbox Protocol is possible via forever-increasing list of Allowed Tokens and Allowed Contracts. By allowing users to access more trade routes, deposits, farms, interactions - the [composability](../../leverage-2.0-is-composable.md) of Gearbox Protocol can really shine! This page is dedicated to keeping an up-to-date list of Allowed Tokens and Allowed Contracts.

{% hint style="success" %}
Gearbox architecture is very modular, so it's not just that there is an allowed asset for the entire protocol - there are different pools and **can even be multiple pools for the same asset**. There can be **different Credit Managers with different Allowed List policies**, etc. The information below is just an easy-to-grasp understanding for product users. Developers should dive into the tech section in Gearbox Dev docs and understand the intricacies. Namely, the tree goes as follows:

* pool
  * credit manager
    * allowed assets
    * allowed contracts
{% endhint %}

If you want to check and see the list of deployed contracts, go here:

{% embed url="https://dev.gearbox.fi/contracts/deployed-contracts" %}

{% hint style="info" %}
If working with the raw numbers, [LT](../liquidations/#liquidation-threshold) for stables would work as follows: a swap from a stablecoin to a stablecoin would cause your [Health Factor](../../traders-and-farmers/credit-account-dashboard-overview/kak-ne-byt-rekt.md#what-i-can-do-if-my-health-factor-is-close-to-1-to-keep-my-credit-account-alive) to majorly decrease, that is because stables are not always stable from the price feed and risks perspective. As such, minor semi-manual assumptions could be made in order to improve user experience, whereas certain select asset types would be granted higher LT. See [GIP-2](https://gov.gearbox.fi/t/gip-2-voting-for-allowed-tokens-list/345) for example.
{% endhint %}

### Allowed Contracts List

* Curve Finance 3pool - [0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7](https://etherscan.io/address/0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7)
* Uniswap V2 - [0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D](https://etherscan.io/address/0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D)
* Uniswap V3 - [0xE592427A0AEce92De3Edee1F18E0157C05861564](https://etherscan.io/address/0xE592427A0AEce92De3Edee1F18E0157C05861564)
* Yearn Finance yUSDC - [0xa354F35829Ae975e850e23e9615b11Da1B3dC4DE](https://etherscan.io/address/0xa354F35829Ae975e850e23e9615b11Da1B3dC4DE)
* Yearn Finance yDAI - [0xdA816459F1AB5631232FE5e97a05BBBb94970c95](https://etherscan.io/address/0xdA816459F1AB5631232FE5e97a05BBBb94970c95)
* Sushiswap - [0xd9e1cE17f2641f24aE83637ab66a2cca9C378B9F](https://etherscan.io/address/0xd9e1cE17f2641f24aE83637ab66a2cca9C378B9F)

{% hint style="success" %}
This was established by the DAO (token holders) and multisig as [part of the first GIPs](https://gov.gearbox.fi/t/gip-3-proposal-for-allowed-contracts/351). Submit to Gearbox DAO your favorite protocol so that [governance](../../governance/setup/) can vote it in!
{% endhint %}

### Allowed Assets List

| Asset  | LT for USDC & DAI                         | LT for WBTC & ETH                     | Address                                    | Price Oracle                               |
| ------ | ----------------------------------------- | ------------------------------------- | ------------------------------------------ | ------------------------------------------ |
| 1INCH  | 77.5%                                     | 77.5%                                 | 0x111111111117dc0aa78b770fa6a738034120c302 | 0x72AFAECF99C9d9C8215fF44C77B94B99C28741e8 |
| AAVE   | 75%                                       | 75%                                   | 0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9 | 0x6Df09E975c830ECae5bd4eD9d90f3A95a4f88012 |
| COMP   | 80%                                       | 80%                                   | 0xc00e94cb662c3520282e6f5717214004a7f26888 | 0x1B39Ee86Ec5979ba5C322b826B3ECb8C79991699 |
| CRV    | 77.5%                                     | 77.5%                                 | 0xD533a949740bb3306d119CC777fa900bA034cd52 | 0x8a12Be339B0cD1829b91Adc01977caa5E9ac121e |
| DAI    | <p>87.5% for USDC,<br>93% for DAI</p>     | 85%                                   | 0x6B175474E89094C44Da98b954EedeAC495271d0F | 0x773616E4d11A78F511299002da57A0a94577F1f4 |
| DPI    | 77.5%                                     | 77.5%                                 | 0x1494ca1f11d487c2bbe4543e90080aeba4ba3c2b | 0x029849bbc0b1d93b85a8b6190e979fd38F5760E2 |
| FEI    | 85%                                       | 85%                                   | 0x956F47F50A910163D8BF957Cf5846D573E7f87CA | 0x7f0d2c2838c6ac24443d13e23d99490017bde370 |
| FTM    | 0.01%                                     | 0.01%                                 | 0x4e15361fd6b4bb609fa63c81a2be19d873717870 | 0x2DE7E4a9488488e0058B95854CC2f7955B35dC9b |
| LDO    | 75%                                       | 75%                                   | 0x5a98fcbea516cf06857215779fd812ca3bef1b32 | 0x4e844125952D32AcdF339BE976c98E22F6F318dB |
| LUNA   | 0.01%                                     | 0.01%                                 | 0xd2877702675e6ceb975b4a1dff9fb7baf4c91ea9 | 0x91E9331556ED76C9393055719986409e11b56f73 |
| LINK   | 75%                                       | 75%                                   | 0x514910771AF9Ca656af840dff83E8264EcF986CA | 0xDC530D9457755926550b59e8ECcdaE7624181557 |
| SNX    | 77.5%                                     | 77.5%                                 | 0xc011a73ee8576fb46f5e1c5751ca3b9fe0af2a6f | 0x79291A9d692Df95334B1a0B3B4AE6bC606782f8c |
| SUSHI  | 77.5%                                     | 77.5%                                 | 0x6b3595068778dd592e39a122f4f5a5cf09c90fe2 | 0xe572CeF69f43c2E488b33924AF04BDacE19079cf |
| UNI    | 75%                                       | 75%                                   | 0x1f9840a85d5af5bf1d1762f925bdaddc4201f984 | 0xD6aA3D25116d8dA79Ea0246c4826EB951872e02e |
| USDC   | <p>87.5% for DAI, </p><p>93% for USDC</p> | 85%                                   | 0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48 | 0x986b5E1e1755e3C2440e960477f25201B0a8bbD4 |
| WBTC   | 85%                                       | <p>85% for WETH, <br>93% for WBTC</p> | 0x2260fac5e5542a773aa44fbcfedf7c193bc2c599 | 0xdeb288F737066589598e9214E782fa5A8eD689e8 |
| WETH   | 85%                                       | <p>85% for WBTC,<br>93% for WETH</p>  | 0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2 | 0x5f4eC3Df9cbd43714FE2740f5E3616155c5b8419 |
| YFI    | 72.5%                                     | 72.5%                                 | 0x0bc529c00c6401aef6d220be8c6ea1667f6ad93e | 0x7c5d4F8345e66f68099581Db340cd65B078C41f4 |
| yvDAI  | <p>87.5% for USDC, <br>90% for DAI</p>    | 85%                                   | 0xdA816459F1AB5631232FE5e97a05BBBb94970c95 | 0x614f9486Ab9C7a217526c097656D2F6bD2DB631C |
| yvUSDC | <p>90% for USDC, <br>87.5% for DAI</p>    | 85%                                   | 0xa354F35829Ae975e850e23e9615b11Da1B3dC4DE | 0x172971182351e00C2D700bA1e8c5586Ad2CFa38c |

**Update #1, 23 December 2021:** DPI forbidden

**Update #2, 18 April 2022:** added FTM, LUNA, CRV, SUSHI, LDO.&#x20;

**Update #3, 12 May 2022:** LUNA, FTM liquidation threshold was changed from 72.5%,72.5% to 0.01%, 0.01%.
