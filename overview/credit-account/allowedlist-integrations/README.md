---
description: Constantly updated list of Allowed Tokens and Contracts.
---

# AllowedList - Integrations

Composability of Gearbox Protocol is possible via forever-increasing list of Allowed Tokens and Allowed Contracts. By allowing users to access more trade routes, deposits, farms, interactions - the [composability](../../../what-can-you-do-with-leverage-2.0.md) of Gearbox Protocol can really shine!&#x20;

Gearbox architecture is very modular, so it's not just that there is an Allowed Asset for the entire protocol - there are different pools and **can even be multiple pools for the same asset**. There can be **different Credit Managers with different Allowed List policies**, etc. Developers should dive into the tech section in Gearbox Dev docs and understand the intricacies.

* Pool
  * Credit Manager
    * allowed assets
    * allowed contracts
* Credit Accounts

The list is mostly kept up-t-date here:

_<> link incoming post deployment <>_

{% hint style="success" %}
The AllowedList is basically a permission box, but within that box - all the actions are permissionless. You decide how to apply leverage, where to apply it, how to trade assets and when. There are no vaults or pre-made strategies here, you can manage it however you want within the Allowed List permissions. Extended dApp can be easier for complex operations. You can, of course, also manage it all fully onchain with your own infrastructure!
{% endhint %}

If you want to check and see the list of deployed contracts, go here:

{% embed url="https://dev.gearbox.fi/" %}
