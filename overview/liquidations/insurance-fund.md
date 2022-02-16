---
description: Protocol-owned reserve fund. The model can be expanded if DAO decides to.
---

# Reserve Fund

{% hint style="info" %}
Even if the math is right on paper, it doesn't always end up so crisp when things come to on-chain execution: high gas fees, bad liquidator work, etc. - can result in the protocol having bad debt and becoming undercollateralized. To prevent it or to retroactively restore capital in such situations, different mechanisms can be put in place. Those include liquidity backstop using governance tokens either by selling them or having LPs do that (like in Aave), having a separate Reserve Fund to pay out liquidity providers (like every CEX has), and so on. Sometimes, these strategies can be combined for extra safety.
{% endhint %}

Gearbox treasury fees accrue in form in LP tokens, instead of idle assets like in most other protocols. As a result, Treasury itself becomes a liquidity provider to the pool. This is like re-supplying liquidity to keep growing - by default - while other protocols usually need to make a separate transaction to turn their idle assets into productive working LP positions.&#x20;

This part of the treasury in form of LP tokens is used to cover losses of the pools in case a the Credit Account is closed with a loss for the pool (bad or untimely liquidation). In such cases, Gearbox Protocol automatically burns their part of the Treasury’s LP tokens - restoring the rate of [Diesel Tokens](../../liquidity-providers/pools-and-apy.md#what-is-a-diesel-token). This way, DAO Treasury acts as Reserve Fund that automatically compensates liquidity providers’ losses up to the level it is physically able to.

Of course, such a design has limitations: the maximum amount of losses compensated by the Reserve Fund is limited by the valuation of LP tokens owned by the DAO Treasury. By default, all payments that DAO Treasury receives from the protocol are made in LP tokens. However, DAO can manage it by withdrawing part of the funds from the pool (thus, instead of LP tokens, Treasury will receive the usual underlying asset of the pool aka idle assets). This way, the DAO can limit itself depending on how much it wants its earnings to be exposed to the Reserve Fund.

{% hint style="warning" %}
This Reserve Fund model doesn't relate to actual software hacks. It specifically covers cases of under-collateralization due to incorrect liquidations. See what [risks](../../risk-and-security/risks-terms.md#protocol-technical-disclosure) there are.
{% endhint %}

Gearbox solves this problem in an elegant way described below.

The concept is described in the Tech Paper:

{% content-ref url="../whitepaper.md" %}
[whitepaper.md](../whitepaper.md)
{% endcontent-ref %}

