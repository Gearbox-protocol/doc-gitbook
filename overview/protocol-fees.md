---
description: To stay self-sustainable, the protocol takes fees for different operations.
---

# Protocol Fees

### **Liquidation Fee**

If a Credit Account is liquidated, some percentage goes to a third-party liquidator who liquidated the account - and some percentage goes to Gearbox Protocol.

* Current liquidation fee going to the liquidator: 4%
* Current liquidation fee going to the protocol: 1.5%

### APY Spread Fee: 50%

The protocol takes spread as a fee between the APY which liquidity providers recieve and the fee & farmers pay for borrowing their assets. The exact value of this fee is calculated as following:

* Each pool has it’s interest rate curve. This interest rate curve represents borrow APY that lenders receive as a function of pool’s utilization r(u). See details and formulas at [dev docs](https://dev.gearbox.fi/docs/documentation/pools/intro/#rt---borrow-apy).
* Borrowers pay borrow APY to liquidity providers and pay spread fee to DAO spreadFee. That means effective borrow rate for borrowers is calculated as r(u)\*(1+spreadFee). DAO receives r(u)\*spreadFee.

{% content-ref url="../liquidity-providers/pools-and-apy.md" %}
[pools-and-apy.md](../liquidity-providers/pools-and-apy.md)
{% endcontent-ref %}

{% hint style="success" %}
All protocol fees go to [governance](../governance/setup/multisigs.md#financial-treasury-multisig-or-5-7) and nothing is assumed for the core contributors or the foundation. The protocol is fully operated by a DAO community.
{% endhint %}
