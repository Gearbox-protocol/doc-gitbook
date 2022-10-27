---
description: To stay self-sustainable, the protocol takes fees for different operations.
---

# Protocol Fees

As mentioned in previous sections, Gearbox Protocol has two sides - lenders ([liquidity providers](../liquidity-providers/pools-and-apy.md)) and borrowers ([traders/farmers](broken-reference)). The protocol is designed to receive fees from both sides:

{% hint style="info" %}
This was established by the DAO (token holders) and multisig as [part of the first GIPs](https://gov.gearbox.fi/t/gip-1-proposal-to-add-pools/347).
{% endhint %}

**Liquidation fee**

If a Credit Account is liquidated, some percentage goes to a third-party liquidator who liquidated the account - and some percentage goes to Gearbox Protocol.

* Current liquidation fee going to the liquidator: 5%
* Current liquidation fee going to the protocol: 2%

#### APY Spread Fee: 50%

The protocol takes spread as a fee between the APY which liquidity providers recieve and the fee & farmers pay for borrowing their assets. The exact value of this fee is calculated as following:

* Each pool has it’s interest rate curve. This interest rate curve represents borrow APY that lenders receive as a function of pool’s utilization r(u). See details and formulas at [dev docs](https://dev.gearbox.fi/docs/documentation/pools/intro/#rt---borrow-apy).
* Borrowers pay borrow APY to liquidity providers and pay spread fee to DAO spreadFee. That means effective borrow rate for borrowers is calculated as r(u)\*(1+spreadFee). DAO receives r(u)\*spreadFee.

{% content-ref url="../liquidity-providers/pools-and-apy.md" %}
[pools-and-apy.md](../liquidity-providers/pools-and-apy.md)
{% endcontent-ref %}

{% hint style="success" %}
All protocol fees go to [governance](../governance/setup/multisigs.md#financial-treasury-multisig-or-5-7) and nothing is assumed for the core contributors or the foundation. The protocol is fully operated by the decentralized community.
{% endhint %}

#### **Liquidity Provider Fees**

A withdrawal fee is taken when a liquidity provider withdraws funds from the pool.&#x20;

* Current withdrawal fee: 1%.

{% hint style="warning" %}
****[**LP withdrawal fee is planned to go away in November. So you can disregard it!**](https://gov.gearbox.fi/t/gip-25-remove-withdrawal-fee/1684)****

Withdrawal fees on the LP side are not considered to be sustainable source of protocol revenue as it creates conflict of interest between the protocols and its LPs. Yearn has previously moved away from this model. In the future, [governance](../governance/setup/) can either implement a performance fee or some other mechanism in order to best align interests.&#x20;
{% endhint %}
