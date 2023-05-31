---
description: Testing the first product with the most degen DeFi users!
---

# Kovan testing with DegenScore & lobsterdao

{% hint style="danger" %}
Initial testing period is now over. A version will be kept available on Kovan for new users to come and test w/o having to incur high mainnet gas fees. Info TBD, stay tuned. Please see this page to learn if you got some GEAR allocated to you for being an awesome member! Snapshot was taken at [Kovan block 28668076](https://kovan.etherscan.io/block/28668076), December 7.
{% endhint %}

{% content-ref url="early-drop.md" %}
[early-drop.md](early-drop.md)
{% endcontent-ref %}

This was the time to give the app into the hands of the most tech-savvy DeFi users: to test the user flow, to understand how degens think, to realize how to improve further... \


{% embed url="https://app.beta.gearbox.fi/" %}

![](../../.gitbook/assets/IMG\_5997.PNG)

{% hint style="success" %}
Gearbox is not a company. Gearbox is not just a product. **Gearbox is a protocol, a DeFi primitive.** But before Gearbox is able to become a composable leverage protocol, a _chicken-and-egg_ problem must be solved: getting liquidity providers as well as traders & farmers to the protocol. This is done with the product approach, see below!
{% endhint %}

{% tabs %}
{% tab title="Code Invite" %}
The codes could be found across Discord, Twitter, or by trying to find contributors and early developers in Paris - where some codes were given in July 2021. It was an exclusive batch, and was given to the most relentless DeFi users from across different communities.

![](<../../.gitbook/assets/Screenshot 2021-08-11 at 00.35.47.png>)
{% endtab %}

{% tab title="DegenScore Apes" %}
DegenScore Citadel and the most vicious DeFi traders could get access to the beta on Kovan. The starting number was at about 700 and then was slightly reduced to allow more testers in. These apes are some of the most savvy users who really could help test the app before the launch.

![](<../../.gitbook/assets/Screenshot 2021-08-11 at 00.36.00.png>)
{% endtab %}

{% tab title="lobsterdao 2+" %}
{% embed url="https://twitter.com/GearboxProtocol/status/1459496426346586112" %}
{% endtab %}
{% endtabs %}

{% hint style="info" %}
The app already contains **HELP (?)** in the bottom right that you can click on for tips.
{% endhint %}

As Kovan is not a live environment, it's harder to run DeFi tests on it. Andre [said it before](https://www.reddit.com/r/yearn\_finance/comments/j2fz77/why\_developer\_andre\_cronje\_tests\_in\_prod/). The liquidity is fragmented and not every protocol is deployed. For a protocol like Gearbox, which puts composability at its core and thus depends on other protocols to function as a lego house, it was a challenge!

So to make the experience as real as possible - or rather, less degraded - we did the following:

* We made new contracts for DAI, WBTC, USDC, and other tokens in order to be able to seed liquidity into Uniswap V2, Uniswap V3, and Sushiswap pools. Have we not done that, any trade would essentially have the slippage at over 10% and make the testing absolutely impossible.
* You could request from the faucet 4 main assets. There was a separate tab for it.
* We made our own arbitrage bot to make trading a bit more realistic, and to also keep the prices among those newly created assets more real. &#x20;
* We made our own liquidation bot which could simulate liquidation if HF was going < 1.

> This was exciting to build! And helped us understand the protocol even better.

{% hint style="warning" %}
It can very well happen that your trade doesn't go through and gives a mistake, or while closing the account it reverts you back. These issues are caused by lack of liquidity on Kovan or maybe by the testing revealing some mistakes in the app logic. Naturally, it's better to know about all of them in advance. So, please, still do [report them](https://discord.gg/pj7xSrp8WE)!
{% endhint %}

## Kovan Testing Step-By-Step

To really test the product, it's better to have users try all the options in different sessions and explore the app in ways which can only be done with having a larger tester base. So here are some instructions:

1. **Start!** Go to the faucet. At least get ETH as you'd need it for gas costs.
2. Try to supply or withdraw liquidity on the "Earn" page. Check those transactions in the block explorer.
3. Open your first Credit Account with the collateral of your choice.&#x20;
4. Try to make some trades, see how the slippage works, see how your health factor changes.
5. Try to change slippage permissions and AMM for execution.
6. Try Wallet Connect feature and execute some trades on native apps of other protocols.
7. Try to open a new Credit Account in another collateral.
8. Try to borrow more if possible or add more collateral.
9. Check your health factor and other stats again.
10. Try to close your Credit Account with either of the options presented.
11. [**Tell in Discord about your experience**](https://discord.gg/pj7xSrp8WE)! Send the bugs, what you liked or disliked about the app, what things worked poorly, what was not clear, and so on. Please be explicit.&#x20;

Here is some information that can help get to your issue as fast as possible:

* include the link to the page where the issue occurred;
* include a screenshot to best explain your issue;
* include browser specifications.

{% embed url="https://discord.com/invite/pj7xSrp8WE" %}
A dedicated Kovan test stage channel.
{% endembed %}

![The work is done for now! Well done ⚙️📦](https://media.giphy.com/media/VbAFrrDVGAvZu/giphy.gif)

{% hint style="info" %}
The instructions are specifically not more clear than this, because the goal is to see how you as a new user would interact and understand the app. That should eventually not require an extra user guide or instructions - but it does at the beginning.&#x20;

**Again, thank you & LFG!**
{% endhint %}
