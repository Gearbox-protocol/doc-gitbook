---
description: Information about guards initiative, also known as multisig signers.
---

# Guards \[Multisigs]

Multisig roles were split into a financial-treasury and technical. Both multisigs were created prior to the deployment ceremony by previous initial core members, as contracts needed to know the wallet addresses. Then, multisig members and a signer count requirement were added after **DAO voting procedures**. All this can be verified on-chain and Etherscan in logs of respective contracts.

{% hint style="info" %}
Multisig must execute whatever proposal reaches winning quorum. Given that multisig are members previously enacted by token holders, meaning the DAO, and are semi-public people with big reputation - in _extreme_ cases they could voice against implementing some proposal. However, that could breach _trust_ in the governance model and require immediate action and restructuring. This must be exercised carefully.
{% endhint %}

## Technical Guard | 6/12

Executes proposals which have reached quorum related to technical changes and the protocol.

Ethereum Address: [0xA7D5DDc1b8557914F158076b228AA91eF613f1D5](https://etherscan.io/address/0xA7D5DDc1b8557914F158076b228AA91eF613f1D5)

List of members on the multisig:

1. [zefram.eth](https://twitter.com/boredGenius) - Building [88mphapp](https://twitter.com/88mphapp), sudoswap, and more. Member of MetaCartel.
2. [Ignacio](https://twitter.com/iicc\_eth) - Co-Founder of Stakely
3. van0k - Gearbox protocol developer
4. [0xmikko](https://twitter.com/0xmikko\_eth) - original inventor of Gearbox \[on behalf of Gearbox Protocol Limited]
5. [Alex Smirnov](https://twitter.com/AlexSmirnov\_\_) - co-founder of [deBridge](https://twitter.com/deBridgeFinance)
6. [MacLane Wilkison](https://twitter.com/MacLaneWilkison) - co-founder of [NuCypher](https://twitter.com/NuCypher) & [Threshold](https://twitter.com/TheTNetwork)
7. [Simone](https://twitter.com/kronosimste) - developer at [DegenScore](https://twitter.com/DegenScore)
8. [Lewi](https://twitter.com/lewifree) - OG degenerate & ESD summoner
9. [Klim](https://twitter.com/milkyklim) - data analytics and [YFI](https://twitter.com/iearnfinance) Maximalist
10. [Alex](https://gov.gearbox.fi/t/multisig-ceremony-apply/95/30) - ex-Neutrino, a lobster and a builder
11. [Alex](https://twitter.com/0xAlexEuler) - CTO of [Mellow Protocol](https://twitter.com/Mellowprotocol)
12. [Lekhovitsky](https://twitter.com/lekhovitsky) - Gearbox protocol developer

{% hint style="success" %}
Transactions related to technical changes and protocol improvements are behind a 2-day timelock, and you can transparently observe every stage and queue in the [Risk Framework](https://risk.gearbox.foundation/updates):&#x20;
{% endhint %}

{% embed url="https://risk.gearbox.foundation/updates" %}

### Veto / Unpause role | 4/12

Ethereum Address: [0xbb803559B4D58b75E12dd74641AB955e8B0Df40E](https://etherscan.io/address/0xbb803559B4D58b75E12dd74641AB955e8B0Df40E)

A multisig with the same set of singers as the Technical Guard, but a lower 4/12 for faster response.

The veto role is related to the ability to circumvent malicious proposals and transactions, it can only say "no" basically, but can't propose or push anything. The unpause role relates to unpausing.

{% hint style="warning" %}
The pause function was granted to [2 analytical addresses](https://gov.gearbox.fi/t/gip-17-multisig-reshuffle-pausable-admin/1447) 1/1. They can only pause the protocol, in case their monitoring tools detect issues, in an attempt to stop the protocol from being fully exploited. In case that is possible and the time onchain gives that window.

* 0xD5C96E5c1E1C84dFD293473fC195BbE7FC8E4840
* 0x65b384cecb12527da51d52f15b4140ed7fad7308
{% endhint %}

***

## Treasury Guard | 5/10

Executes proposals which have reached quorum related to spending, grants, and the treasury overall.

Ethereum Address: [0x7b065Fcb0760dF0CEA8CFd144e08554F3CeA73D1](https://etherscan.io/address/0x7b065Fcb0760dF0CEA8CFd144e08554F3CeA73D1)

List of members on the multisig:

1. [Stani](https://twitter.com/StaniKulechov) - founder of [Aave](https://twitter.com/AaveAave), venture partner at [Variant Fund](https://twitter.com/VariantFund)
2. [Amplice](https://twitter.com/astr0bas3d) - [lobsterdao](https://twitter.com/10b57e6da0) member & core DAO contributor on marketing
3. [Pepo](https://twitter.com/0xPEPO) - contributor of [Wonderland](https://twitter.com/defi\_wonderland) & [DeFi LATAM](https://twitter.com/defi\_latam)
4. [Sergey](https://t.me/icodrops\_sergey) - founder of [ICODrops](https://twitter.com/ICODrops)
5. [NDW](https://twitter.com/cryptondee) - Castle Capital member and a DeFi degen
6. [apeir99n](https://twitter.com/apeir99n) - original math & product at Gearbox \[on behalf of Gearbox Protocol Limited]
7. [Nikitakle](https://twitter.com/NOstroymov) - core DAO contributor on marketing & community
8. [Amantay](https://gov.gearbox.fi/u/amantay/summary)  - core DAO contributor on risk & analytics
9. [duckdegen.eth](https://twitter.com/DuckDegen) - devrel, ex-Connext \[[GIP-40](https://gov.gearbox.fi/t/gip-40-financial-multisig-reshuffle/2204/5)]
10. [Vadym](https://twitter.com/0x\_vadym) - head of product at Kolibrio

Spending and grants paid out can be seen in monthly DAO reports:

{% embed url="https://gearboxprotocol.notion.site/Monthly-Reports-6849871a9bae44dfb903531c0a997e8f" %}

### Fee Temporary Guard 5/10

Ethereum Address: [0x3E965117A51186e41c2BB58b729A1e518A715e5F](https://etherscan.io/address/0x3E965117A51186e41c2BB58b729A1e518A715e5F)

A temporary multisig with the same set of singers as the Treasury Guard. It is created to separate funds from the [DAO rounds](../../gear-token/supply-information.md#early-backers-and-dao-round-2022) which are used for the development of the protocol. This Fee Guard collects all [fees from the protocol](../../overview/protocol-fees.md) and can later on give control over to an initiative which will focus on staking programs, or whatever else the DAO decides to do. It's a holder of fees for now.
