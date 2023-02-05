---
description: The path to decentralization and community governance from summer 2021.
---

# DAO-First Launch

_Gearbox is not just a product. Gearbox is a protocol, a DeFi primitive._&#x20;

The liquidity and trading are not siloed within the protocol. The goal is to be composable and open. And if that is the case, so should be the information and control over the protocol! This page is dedicated to the historical events about how Gearbox has progressed to launch.&#x20;

### Initial core members and contributors&#x20;

January - August 2021: getting the tech paper, architecture, and everything together.

{% content-ref url="birth-at-ethglobal-marketmake-and-first-contributors.md" %}
[birth-at-ethglobal-marketmake-and-first-contributors.md](birth-at-ethglobal-marketmake-and-first-contributors.md)
{% endcontent-ref %}

August-November 2021: educating the community to prepare to ship control over the protocol. As well as audits and security testing for the core contracts prior to launch in December 2021.&#x20;

{% content-ref url="kovan-testing-with-degenscore.md" %}
[kovan-testing-with-degenscore.md](kovan-testing-with-degenscore.md)
{% endcontent-ref %}

See how the product has evolved over 2021 while being tested:&#x20;

{% embed url="https://medium.com/gearbox-protocol/product-evolution-from-an-idea-to-an-app-0-to-1-contributors-united-832154e3c7ba" %}

### DAO Taking Over - December 2021&#x20;

{% embed url="https://youtu.be/szg_CvrxU9w?t=10155" %}

The DAO-first launch model was proposed during ETHGlobal Online event. You can watch the long version of the presentation on youtube, starting from 2:49:15.&#x20;

What is the TLDR for DAO-first? It's that the previous "team" (initial core members) ship the code open-source and retain no control over the protocol even from day -1. That's right: not deciding on collaterals, not deciding on allowed policy list, etc. **All of that goes through the DAO voting and multisig implementing it, where previous team and contributor votes / signatures are a minority**.&#x20;

#### 1. Token distribution and genesis contracts deployment

{% embed url="https://etherscan.io/address/0x20da9f3d7d5cb96c2822338830cfd6dee6d508d8" %}
Gearbox Core V1 Deployer
{% endembed %}

In order to have the community take over and be able to operate the protocol, the initial distribution had to be done in a very diverse way: committed contributors & coders, initial users who took their time to analyze the protocol and help improve it, and so on. After all, these are the holders who will be deciding the future of Gearbox! For example, honoring early community:

{% content-ref url="early-drop.md" %}
[early-drop.md](early-drop.md)
{% endcontent-ref %}

You can see that overall the distribution of [GEAR](broken-reference) took place across several phases!

{% embed url="https://medium.com/@gearboxprotocol/gear-token-not-yet-live-and-governance-reverse-voting-escrow-75f367985397" %}

{% hint style="info" %}
At this stage, most of the core contracts were deployed but were open-sourced just yet. Only the ones necessary for this stage to be verified. The tokens were by default not transferrable by anyone except the distributor. Later on, DAO could make a decision to make tokens transferrable, or decide to never do it.&#x20;
{% endhint %}

#### 2. Credit Account Mining&#x20;

This was one of the stages related to token distribution for the community side. With a twist!

You see, users need to rent [Credit Accounts](../credit-account/) from Gearbox Protocol when accessing composable leverage. Why? Because deploying and throwing away SC every time is a costly and sad procedure. But so is deploying 5,000 isolated smart contracts - it's very costly... and it's not fun to do it just as core team! Thus, a more engaging community-inspired model was designed.&#x20;

A designated list of wallets, that took part in governance of many other protocols previously, could pay gas costs on mainnet to deploy one account per wallet - and receive fixed amount of GEAR.&#x20;

The snapshot was taken and discussed with the community to analyze for the traits of sybil in other protocols. The list could not be perfect, but it's about making sure that the majority of real members could take part, even if some botting could occur. Learn all about it:

{% content-ref url="credit-account-mining.md" %}
[credit-account-mining.md](credit-account-mining.md)
{% endcontent-ref %}

#### 3. Treasury Multisig & Technical Multisig | Delegators

The roles of multisigs were set up to a financial-treasury one (receiving protocol fees, paying grants, holding DAO portion of GEAR tokens) and a technical one (implementing technical changes according to outcomes of voting, setting up parameters, and executing other technical protocol tasks). Both multisigs were voted in by the diverse list of token holders - assigned up to this stage. Technical multisig naturally has a higher signer majority count.&#x20;

Delegates were set up at this stage to streamline community work & power.

{% content-ref url="../../governance/setup/guards-multisigs.md" %}
[guards-multisigs.md](../../governance/setup/guards-multisigs.md)
{% endcontent-ref %}

{% hint style="info" %}
At this point, the initial core team no longer had control over the protocol. The community took over all of the operations and had the major vote and handled further operations. Initial core team stops existing as a concept, and DAO takes over as the main boss.
{% endhint %}

#### 4. Voting for pools, parameters, and allowed lists&#x20;

Core members were not in charge of deciding of what assets and protocols are first to be on Gearbox [AllowedList](../credit-account/#allowed-list-policy). Every financial parameter (collaterals, assets, protocols, liquidation thresholds, other parameters) were to be decided by the DAO with a minimum quorum. The discussions included forum proposals for temperature check, followed by snapshot page voting.

{% embed url="https://gov.gearbox.fi/t/template-proposal-for-managing-gearbox-protocol-parameters/100" %}

#### 5. Final deployment and launch on mainnet&#x20;

Technical multisig took over all the decisions of the step 4 and implemented them in [code](https://twitter.com/mikaellazarev/status/1473322250149539842?s=20). All the contracts were open-sourced and verified on Etherscan. The protocol was deployed and launched.&#x20;

{% embed url="https://discord.com/invite/jJuABVH9Pg" %}
That's it. The rest is history. GLHF!
{% endembed %}

{% embed url="https://youtu.be/JJQPyJ9BKgM" %}

{% hint style="success" %}
Ahhhh i am a governooooor... but for real, [join and contribute](broken-reference)! Let's build together <3
{% endhint %}

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}
