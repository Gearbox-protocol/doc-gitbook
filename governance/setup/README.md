---
description: 'Early governance: forum + snapshot + multisigs.'
---

# Governance Model

{% hint style="info" %}
****

**Where is the DAO, how can I contribute?**

You can be in a DAO but not be 24/7 active, which is totally okay. There are different ways to get involved and get rewarded for your time and skills.&#x20;

* **Core contributors**: those who day and/or night work on different tasks as core contributors, ranging from marketing to coding. DAO contributors are split among different sub-projects and can decide to work on something specific, or a few tasks at a time. [See Notion](https://gearboxprotocol.notion.site/Gearbox-DAO-23966f122ae4421492819242b30a0e7a).&#x20;
* **Delegates**: members who stay on top of protocol strategic ideas and plans, but don’t have the 24/7 to really get hands-on operational tasks. They can become delegates and lead how [governance](./) decides on protocol vital things.&#x20;
* **Shitposters**: you can meme, learn, and discuss DeFi in [Discord](https://discord.com/invite/gearbox). We’ll like you ;)
{% endhint %}

{% embed url="https://gearboxprotocol.notion.site/Gearbox-DAO-23966f122ae4421492819242b30a0e7a" %}

Gearbox Protocol did not have a core team from day 0, no central authority! Initial members handed over the code to the DAO who then deployed the protocol and even decided the initial pools, assets, collateral types, and so on. The DAO consists of the community multisigs and a few hundred of token holders as per the **DAO-First Launch** strategy. Snapshot + multisigs is used.

![](<../../.gitbook/assets/Screenshot 2021-10-18 at 21.23.24 (1).png>)

_Governance is one of the most complex things which requires tedious research. MakerDAO, Element Finance, Yearn, Coordinape and other protocols have advanced this process forward also by making data on voter apathy and activity. The goal is to figure Gearbox governance step-by-step and have users be in control of the protocol. Have the community decide and iterate!_

{% hint style="success" %}
You can [discuss governance models on Discord](https://discord.gg/kPejWrzfTw) and [governance forum](https://gov.gearbox.fi/c/main/). See [Notion](https://gearboxprotocol.notion.site/gearboxprotocol/Gearbox-DAO-Working-Sheet-23966f122ae4421492819242b30a0e7a).
{% endhint %}

Protocols should be given away to communities as soon as possible, to let a movement start from the roots. But with such a decision comes big responsibility - ensuring proper and adequate governance rails for new members to coordinate, judge things, and decide on the future. And while fully on-chain governance models like [Governor Alpha](https://medium.com/tally-blog/the-case-for-governor-alpha-15c1362d49eb) are seen as one of the staples that projects should aspire to - it's practically impossible to achieve that in the first weeks of a protocol life, because there are so many unknowns with regard to PMF, pools, and other factors.&#x20;

Given that, Gearbox Protocol governance DAO was set up in a flexible yet accountable way, innovating on some of the features to ensure a more streamlined environment.&#x20;

{% hint style="info" %}
It's important to note that all distribution vestings and other parameters were hard-coded in smart contracts no ensure no requirement for trust from day 0. Everything communicated was in code, verified, and audited. But make sure to know the [risks](../../risk-and-security/risks-terms.md).
{% endhint %}

#### PROPOSAL TEMPLATE

{% embed url="https://gov.gearbox.fi/t/template-proposal-for-managing-gearbox-protocol-parameters/100" %}

## Governance discussion process

**1. Ideation process, usually in Discord.**

This can occur in any chat really. Discord, forum, wherever. It's best to outline the voting parameters (WHAT are you actually voting for: YES or NO question, for instance) during this process so you would have a better understanding of what to propose on forum.

{% embed url="https://gearboxprotocol.notion.site/gearboxprotocol/Gearbox-DAO-Working-Sheet-23966f122ae4421492819242b30a0e7a" %}
DAO working groups and coordination
{% endembed %}

**2. Forum proposal and temperature check: first in Main, then in Proposals.**

After some initial feedback for an idea was received informally, a semi-formal proposal must be put on forum with concrete explanation of the proposed idea. A temperature check can be used on forum via a voting poll. Such things can easily be gamed, of course, so this temperature check should be met with a degree of scrutiny.&#x20;

{% embed url="https://gov.gearbox.fi/t/start-here-forum-rules/17" %}

**3. Actual formal proposal on snapshot.**&#x20;

It should be put up for voting on the snapshot page, including the transaction details the DAO would be voting for, to avoid any multisig subjectivity later. This means that a proposer should seek technical help to prepare such a transaction prior to submitting a snapshot proposal. A quorum must be bet in such case.

{% embed url="https://snapshot.org/#/gearbox.eth" %}

**4. Multisig execution.**

Multisig must execute whatever proposal reaches winning quorum. Given that multisig are members previously enacted by token holders, meaning the DAO, are semi-public people with big reputation - in _extreme_ cases they could voice against implementing some proposal. However, that could breach _trust_ in the governance model and require immediate action and restructuring.&#x20;

{% hint style="info" %}
[Discord](https://discord.gg/kPejWrzfTw) and [governance forum](https://gov.gearbox.fi/c/main/). Also see [Notion](https://gearboxprotocol.notion.site/gearboxprotocol/Gearbox-DAO-Working-Sheet-23966f122ae4421492819242b30a0e7a).
{% endhint %}

## Initial Governance Specifications

### Reverse Voting Escrow: reducing voting weights of initial core members & initial contributors

![](<../../.gitbook/assets/Screen Shot 2021-12-10 at 19.29.49.png>)

While it's not unnatural for initial core members and contributors to have larger token percentages than regular smaller users (either by early investment, or by early farming, or by just being richer) - it is however a problem for early governance. If small holders have no opportunity to coordinate and price out the larger holders together - governance can be seen as flawed. As such, Gearbox DAO in the early stages - thanks to snapshot mechanics - evens out the playing field by making sure community members have higher voting power than early members.&#x20;

So two issues needed to be fixed:

1.  Whale portions dominating governance as voters;

    Fix -> community delegators to unite small holders.
2.  Whale portions delegating and still dominating;

    Fix -> limit governance weights of whales completely.

The distribution had a few portions:

1. Community members including Credit Account Mining and other portions: full x1 multiplier.
2. Contributors A meaning initial core members: multiplier of x0.125
3. Contributors B meaning initial contributors: multiplier of x0.25
4. Company wallet: cannot vote on anything before and if the governance model changes.
5. DAO wallet: cannot vote unless it gives grants to people, which then gets x1 multiplier.

![](<../../.gitbook/assets/2021-12-10 22.06.43.jpg>)

This way, **community voices are over x2 bigger in its voting power than early contributors and initial core members combined**! According to that, the DAO portion can really be counted as a community portion because of who practically gets to decide what to do with it, whereas neither early group can push anything at their own free will. Avoiding situations of the misuse of power.

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

### Delegation is available to streamline community work

Snapshot page delegation is turned on for delegators from the community to unite and allow smaller holders get their voice. Anyone can delegate to any delegator or multiple delegators at once, including initial core members and contributors. But their votes are reduced, to even out the playing field. See the point above for all the details. This is done on the snapshot page.

{% content-ref url="../community-delegates.md" %}
[community-delegates.md](../community-delegates.md)
{% endcontent-ref %}

### A minimum of 3 days period must be selected on the snapshot

In order to ensure enough time for voting to be done fairly, a 3 day period must be ensured at minimum - with a maximum of 7 days in case the proposal requires that long. Given that prior to a snapshot vote a proposal must be discussed publicly on forum, there is practically more time for one to engage and be prepared to case their vote.

### Minimum 0.02% of total supply to make a snapshot proposal

In order to avoid spam proposals and governance distortion at the snapshot level - and to not cause subjective issues when a proposal is removed for being spammy (which is a subjective matter, and subjectivity must be removed as much as possible) - a minimum of 0.02% of total supply of GEAR are required to make a snapshot proposal.&#x20;

{% hint style="info" %}
At the valuation of 100M that is 20K USD worth and at valuation of 1B that is 200K USD.
{% endhint %}

### A winning vote must also have > 2% total supply quorum

That is a number required in support for a proposal choice in order to classify as legitimately winning, and not the participation in a vote in total.

{% hint style="info" %}
In terms of eligible votes percentage, you need to subtract the DAO portion (51%) and company wallet (11%), as well as reduce early contributors voting weights. Given that initial core members voting weights are being reduced from 20%->2.5% and initial contributors from 9.20%->2.3% - it is almost impossible for early members to pass whatever they want on their own. As such, it is about 2% from the 12% of the available votes, so a 17% quorum of eligible votes for a winning vote. **Community having over 8% is the deciding factor**.
{% endhint %}

{% hint style="warning" %}
A working idea: since it's technically impossible to vote for something like "let's never vote for X again" as such proposals make no sense - a cool-off period of 2 weeks can be established if a proposal went live but did not reach quorum.
{% endhint %}

### Company wallet is not allowed to vote&#x20;

While contributor wallets can vote according to their reduced multiplier, company wallet is not allowed to vote at this stage. Once the vesting starts happening and tokens change hands, new owners would naturally be able to vote. However, that is over 1 year away from launch.

{% hint style="warning" %}
DAO can always decide to lower or increase the quorum or proposal minimum threshold.&#x20;

Proposals on the forum which violate basic human decency like "let's cause damage to someone" can be removed by forum admins, among which community members are. However, proposals which seem weird to some - but do not cause any hard or violence - cannot be removed, as there is no subjectivity allowed when moderating an open forum.

If a snapshot vote was not submitted correctly, for example less than 3 days window for voting - it technically does not count as legitimate and can be taken down by snapshot page admins (the DAO). It is always better to ask for guidance in Discord about how to properly present the voting choices in order to make sure it is worded correctly.
{% endhint %}



## Practical point with regard to the snapshot

{% embed url="https://snapshot.org/#/gearbox.eth" %}
gearbox.eth
{% endembed %}

Given that snapshot voting is off-chain (yet trustless and verifiable) - some parameters allow for flexibility, which is how such a model as described above is possible. However, that also means there is a degree of human intervention required in order to facilitate this.&#x20;

#### Admin role to update multipliers of the reduced voting weights

The weights, as described, shift higher for A and B in case the DAO does more distributions. That is to replicate the fact that DAO ensures more distributions and grants, and as such it's acceptable to have early contributors voting weights increase to their normal level slowly as the community portion increases. However, a few points need to be taken into account:

* What happens after 1 year, when vesting begins? If a new governance system is introduced then, to take into account liquid tokens only, then there will be a period when initial core members and contributors have close to 0% voting weights, which makes it dangerous. So a new system should take a few months period into consideration.
* What if a new system is implemented about half a year into the protocol life, how will the weights be adjusted then? The DAO should be able to vote and find an equilibrium in that case, to balance out the weights. As long ad the original ethos of having a level playing field is maintained (prior to a fully unlocked supply model) - it should be acceptable.

As such, the weight multiplier from x0.125 will be manually updated monthly at the snapshot level to replicate this Reverse Escrow Model change when needed. However, in the first weeks, this action is not necessary as the portions won't drastically change.

{% hint style="info" %}
Because some parameters have to be adjusted at the snapshot level, like total number to calculate quorum - a deviation of 3-5% from the available number (which is less than 1% of overall power) here and there can happen, in order to avoid daily multisig work. As such, bi-weekly or monthly can be chosen in order to keep the numbers in check.
{% endhint %}
