---
description: Protocol-owned reserve fund. The model can be expanded if DAO decides to.
---

# Reserve Fund

[Protocol fees](../protocol-fees.md) accrue in form in [dTokens](../../lending-market/pools-and-apy/#pool-tokens-staked-diesel-tokens), instead of idle assets like in most other protocols. As a result, Treasury itself becomes a passive lender to the pools. This is like re-supplying liquidity to keep growing - by default - while other protocols usually need to make a separate transaction to turn their idle assets into productive working LP positions.&#x20;

By default, accrued fees are used to cover losses of the pools in case a the Credit Account is closed with a loss for the pool (bad or untimely liquidation). In such cases, Gearbox Protocol automatically burns its part of the Treasury’s dTokens - restoring the rate of [Diesel Tokens](../../lending-market/pools-and-apy/#what-is-a-diesel-token). This way, it acts as Reserve Fund that automatically compensates liquidity providers’ losses up to the level it can.

{% hint style="success" %}
By default, all fees that the DAO receives from the protocol are made in LP tokens. However, DAO can manage this by unwrapping part of the funds from the pools (thus, instead of dTokens, DAO will receive the usual underlying asset of the pool aka idle assets). This way, the DAO can limit itself depending on how much it wants its earnings to be exposed.
{% endhint %}

Essentially the Gearbox dTokens inside this Fee Guard are the Insurance Fund. Anything that is not in dTokens has likely been voted to be unwrapped and kept as non Insurance Fund. Any non-dTokens are not counted towards the Insurance Fund size. And this only applies to V3 contracts.

> [https://debank.com/profile/0x3e965117a51186e41c2bb58b729a1e518a715e5f](https://debank.com/profile/0x3e965117a51186e41c2bb58b729a1e518a715e5f)

{% hint style="warning" %}
This Reserve Fund model doesn't relate to actual software hacks. It specifically covers cases of under-collateralization due to incorrect liquidations. See what [risks](../../risk-and-security/risks-terms.md#protocol-technical-disclosure) there are.
{% endhint %}
