---
description: To stay self-sustainable, the protocol takes fees for different operations.
---

# Protocol Fees

As mentioned in previous sections, Gearbox Protocol has two sides - lenders ([liquidity providers](../liquidity-providers/pools-and-apy.md)) and borrowers ([traders/farmers](broken-reference)). The protocol is designed to receive fees from both sides:

### **Liquidity Provider Fees**

A **withdrawal fee** is taken when a liquidity provider withdraws funds from the pool.&#x20;

* Current withdrawal fee: 1%.

{% hint style="warning" %}
Withdrawal fees on the LP side are not considered to be sustainable source of protocol revenue as it creates conflict of interest between the protocols and its LPs. Yearn has previously moved away from this model. In the future, [governance](../governance/setup/) can either implement a performance fee or some other mechanism in order to best align interests.&#x20;

Because Gearbox Protocol currently has TVL caps in place, lack of liquidity can create discrepancies in borrow APY and thus degrade the experience for traders and farmers. Withdrawal fees are in place and shall be removed by governance in a few weeks. This is not the source of protocol revenue, it's simply there as a backstop against system turbulences in the first weeks post-launch.
{% endhint %}

### **Trader / Farmer Fees**

**Liquidation fee**: if a Credit Account is liquidated, some percentage goes to a third-party liquidator who liquidated the account - and some percentage goes to Gearbox Protocol.

* Current liquidation fee going to the liquidator: 5%
* Current liquidation fee going to the protocol: 2%

{% hint style="success" %}
This was established by the DAO (token holders) and multisig as [part of the first GIPs](https://gov.gearbox.fi/t/gip-1-proposal-to-add-pools/347).
{% endhint %}

### APY Spread Fee

The protocol takes spread as a fee between the APY which liquidity providers receive and the fee traders & farmers pay for borrowing their assets. More information is on the Pools & APY page:

{% content-ref url="../liquidity-providers/pools-and-apy.md" %}
[pools-and-apy.md](../liquidity-providers/pools-and-apy.md)
{% endcontent-ref %}

{% hint style="success" %}
All protocol fees go to [governance](../governance/setup/) and nothing is assumed for the core contributors or the foundation. The protocol is fully operated by the decentralized community.
{% endhint %}
