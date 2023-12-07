---
description: DeFi Primitive for composable leverage 2.0
---

# Credit Accounts

![](<../../.gitbook/assets/Screenshot 2021-08-07 at 22.49.38.png>)

A Credit Account is an isolated smart contract which contains both the user funds and the borrowed funds. This is where your leverage is. After you open an account, all the operations go through this account and the assets stay on it as well. You can see a Credit Account as your automated DeFi wallet where you not only keep positions, but can also potentially program it the way you want. _You can at all times see transactions and assets on Etherscan, obviously._

![](<../../.gitbook/assets/Screenshot 2021-08-07 at 23.07.53.png>)

Funds on Credit Accounts are used as collateral for debt, and users can operate these funds by sending financial orders to their Credit Accounts. That could be: margin trading on Uniswap or Sushiswap; leverage farming on Yearn; arbitraging pegged assets on Curve, and more!

See the list of [integrations](../integrations/).

## Allowed List policy

Operations available to users are restricted by two policies:

* **Allowed contracts list**. Users can interact through Credit Accounts only with contracts from this list to mitigate risks that funds will be sent to vulnerable smart contracts.
* **Allowed tokens list**. This allows managing risks of swapping funds to highly-volatile assets whose price could drastically fall after a swap and before a liquidation would take place. Another attack vector is a user creating some dummy ERC20 and then buying it on, let's say' Uniswap - and essentially draining capital from Gearbox Protocol.

Both policies are managed by [governance](../../governance/setup/) and can grow to enable more assets and protocol.

{% content-ref url="allowedlist-policy/" %}
[allowedlist-policy](allowedlist-policy/)
{% endcontent-ref %}

Gearbox architecture is very modular, so it's not just that there is an allowed asset for the entire protocol - there are different pools and **can even be multiple pools for the same asset**. There can be **different Credit Managers with different AllowedList policies**, etc. The information below is just an easy-to-grasp understanding for product users. Developers should dive into the tech section in Gearbox Dev docs and understand the intricacies. Namely, the tree goes as follows:

* Pool
  * Credit Manager
    * allowed assets
    * allowed contracts
* Credit Accounts

{% embed url="https://dev.gearbox.fi" %}

## Low Overhead on Gas

Due to the architecture and design of Gearbox Protocol being modular, users each have their own Credit Account(s) instead of executing trades via a giant joint pool of liquidity with virtual balances of each user (how protocols usually do). Therefore, the gas costs overhead is minimized.&#x20;

Next to that, Credit Accounts are not deployed by users every time as separate smart contracts, but are "borrowed" from the protocol by users like if you were to get an Uber: you use a car and then give it back once finished. This way, the deployment costs are kept to zero for new users.
