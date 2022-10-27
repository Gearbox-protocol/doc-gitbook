---
description: Closing your account and avoiding liquidations.
---

# How to close a Credit Account

{% hint style="success" %}
If you don't want to keep the assets from the Credit Account but just want to close - the best way is to trade out of your positions manually within your Credit Account, and then simply close the Account without the need to use any extra funds. This way, when manually selling assets to the underlying, you can do so slowly and account for low slippage. Then the protocol will simply subtract your debt and return the rest.
{% endhint %}

Before you close a Credit Account, the protocol would want you to pay back what you own. That is the loan you took and the interest accrued to it over the time you used the Credit Account. You can see this amount in the [Credit Account Dashboard](./) section. There are two options to pay back:&#x20;

* Use the Credit Account's funds to repay the debt by automatically swapping all positions inside it to the underlying asset, from which the debt (notional loan + interest accrued) are subtracted and then the difference is given back to you. The better you traded, the more you will get.
* Use your own funds to repay the debt in the underlying asset - and get all the assets from the Credit Account back to your wallet. You essentially prepay the debt, and then the Credit Account releases all the funds on its balance to your personal wallet.

{% hint style="info" %}
**Option number two is preferred in case you really like the assets** you have on your Credit Account and don't want to trade there-and-back and just want to keep the assets. Remember that keeping passive positions on a Credit Account still accrues the interest.

Another reason why **option number two is preferred is because you as a user can slowly trade out of the positions instead of market-selling them**. In case your positions are large, some of the assets on your Credit Account could incur high slippage which the protocol will not allow you to perform such an action and will require you to input larger slippage tolerance.
{% endhint %}

**Step 1.** Click _Manage_ button on your Credit Account's page.&#x20;



{% hint style="danger" %}
Trading LP tokens on the market is not so easy, so make sure to unwrap them yourself. This way, you can avoid harsh slippage and save on liquidator fees. If you LPed into Yearn or another protocol which gives back such asset, you are better off unwrapping manually.
{% endhint %}

## Option 1:  **Swap all assets to the underlying and repay the debt**

The protocol will exchange all the non-underlying asset funds to the underlying asset on DEXes and repay your debt. You will receive the remaining funds to your personal wallet.

{% hint style="warning" %}
The current basic functionality only allows swaps for this feature on Uniswap V2, in which case some assets could incur high slippage. Consider swapping manually.
{% endhint %}

**Step I-1.** Click _Close_ button

<figure><img src="../../.gitbook/assets/Close credit account.png" alt=""><figcaption></figcaption></figure>

**Step I-2.** Choose the maximum size of the slippage that you will tolerate in the options page in the top right corner, and click _Swap and get tokens_ button. If the price falls by more than the slippage while your trade is being confirmed, the trade will be reverted.

<figure><img src="../../.gitbook/assets/screenshot-app-goerli-gearbox-fi-accounts-0x2ad4a2f1bdd815e285a22cdcc072fbb-1666402379978.png" alt=""><figcaption></figcaption></figure>

## Option 2: **C**lose a Credit Account using your funds to decrease the debt

You repay the loan with your own funds. This means you have more funds on your personal wallet. After repayment is done, the assets which were on your Credit Account will be sent to your wallet.

{% hint style="info" %}
This option is possible only if your wallet balance in the denominated asset is at least of the amount required for repaying the debt.
{% endhint %}

**Step II-2.** Click _Decrease Debt_ button in the Manage page.

<figure><img src="../../.gitbook/assets/Decrease Debt.png" alt=""><figcaption></figcaption></figure>

**Step II-2.** Check amount to be repaid and click _Repay_ button

{% hint style="info" %}
Did you find a bug with the interface, something didn't work as you think it should have, or you have a suggestion on how to improve the user experience? [Report](https://discord.gg/5YuHH9tvms) or [suggest](https://discord.gg/hF3QvX2vgt) on Discord!
{% endhint %}
