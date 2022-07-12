---
description: Taking advantage of a correlated asset de-peg.
---

# Arbitrage of correlated assets

When one of the correlated assets de-pegs and you believe the peg will be restored, you can take a leveraged position and arbitrage the difference in price between those assets. Let's imagine DAI > USDC.&#x20;

DAI: $1.05\
USDC: $1.00

1. Go to the [Credit Accounts](https://app.gearbox.fi/) app page.
2. Open a DAI-denominated Credit Account. For example, 100.000 x 10 leverage = 1M DAI.
3. Swap all the DAI from your Credit Account to USDC.
4. Wait until the price of DAI returns to peg of 1:1.
5. Close your Credit Account and fix profits.&#x20;

Not taking slippage and interest rate into account, 1M DAI swapped to USDC at the price of $1.05 would be 1.05M USDC and when closing the account - essentially 50K profits in arbitrage.&#x20;

Same strategy works for the case DAI < USDC. The only difference is that you should open a Credit Account denominated in USDC. Such strategy also can apply to WBTC, or other pegged assets. [Open Credit Account and try it](https://app.gearbox.fi/).

![Flash loans make it possible to arbitrage a peg within one block. Gearbox allows you to do so even if it takes more time. However, with stablecoins it's generally easier as there are other avenues to borrow from. But not for all pegged assets!](<../../.gitbook/assets/Screenshot 2021-10-19 at 00.42.00 (1).png>)

{% content-ref url="../how-to-open-account.md" %}
[how-to-open-account.md](../how-to-open-account.md)
{% endcontent-ref %}

{% hint style="info" %}
Keep in mind that sometimes de-peg can continue for very long or never restore. You as a trader-farmer take all the risks involved. Learn more about the disclosure on [risks](../../risk-and-security/risks-terms.md).
{% endhint %}
