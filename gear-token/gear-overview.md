---
description: GEAR token contract and distribution information.
---

# GEAR Overview

GEAR token is an ERC20 utility token, starting off as a governance token for the protocol - and then possibly taking any other new function the DAO could envision for it. The supply of GEAR is capped at 10,000,000,000 (10 billion) which can't be technically changed. See that in source code.

Token contract: [0xba3335588d9403515223f109edc4eb7269a9ab5d](https://etherscan.io/token/0xba3335588d9403515223f109edc4eb7269a9ab5d)\
Decimals: 18\
Symbol: $GEAR

{% hint style="info" %}
GEAR token started as non-transferrable. That can be changed by DAO voting.
{% endhint %}

## GEAR Distribution

{% hint style="success" %}
Anybody who is not a community member is locked for a minimum of 1 year since launch. All of the vestings can be verified on-chain, no trust required. Community retains the largest portions both in terms of the distribution and in terms of voting weights.

**You can check those by going to the TokenDistributor contract**:

* check contributorsList \[2] to find yourself/someone;
* fill in your/eligible address from \[2] into \[10] vestingContracts. That will give you the corresponding personal vesting contract for that address;
* you can also check \[12] and \[13] for the weight multiplier. For example, if it's 1250 - that means it's x0.125 - this is the reduction early contributors get. FYI, Contributor A = early contributors, Contributor B = initial core members and initial external.
{% endhint %}

{% embed url="https://etherscan.io/address/0xbf57539473913685688d224ad4e262684b23dd4c#readContract" %}
[https://etherscan.io/address/0xbf57539473913685688d224ad4e262684b23dd4c#readContract](https://etherscan.io/address/0xbf57539473913685688d224ad4e262684b23dd4c#readContract)
{% endembed %}

GEAR supply has been split according to a handful of contributor groups:

![Early community maintain majority of voting power. See governance page.](<../.gitbook/assets/Screen Shot 2021-12-10 at 18.26.31.png>)

{% embed url="https://medium.com/@gearboxprotocol/gear-token-not-yet-live-and-governance-reverse-voting-escrow-75f367985397" %}

### Community Portion: 58%. No vesting.

* **DAO Treasury Multisig**: 51.00%. Liquid as the DAO decides. No vesting, managed by the DAO-enacted treasury multisig. Address[: 0x7b065fcb0760df0cea8cfd144e08554f3cea73d1](https://etherscan.io/address/0x7b065fcb0760df0cea8cfd144e08554f3cea73d1)
* **Credit Account Mining**: 5%. Split over 5,000 wallets participated in the ceremony. No vesting.

{% content-ref url="../overview/launch-phases/credit-account-mining.md" %}
[credit-account-mining.md](../overview/launch-phases/credit-account-mining.md)
{% endcontent-ref %}

* **Community Testers**: 1.267%. No vesting. _Token distributor TBA._
* **Early Discord members**: 0.476%. No vesting. _Token distributor TBA._

{% content-ref url="../overview/launch-phases/early-drop.md" %}
[early-drop.md](../overview/launch-phases/early-drop.md)
{% endcontent-ref %}

* **Temporary Reserve**: approximately 0.26%. No vesting. _Token distributor TBA._ \
  __As we set on to a few stages of the community distribution, we expect there could be some technical difficulties with some claimants, or an extra amazing contributor pops up, and so on. This is just a buffer made available for the first few weeks, in case some distributions need to be adjusted. Address -&#x20;

### Initial External Contributors: 1.28%. Locked > 1 year + vesting.

These are some amazing people who have contributed to the technical development and project growth but weren't committing capital, yet we wanted to incentivize them to work further with the DAO. Lockup: 12 months since token deployment (launch), and then linear vesting over 18 months starting after the cliff.&#x20;

### Initial сore contributors: 29.20%. Locked > 1 year + vesting.

**Initial core members 20%** (usually referred to as "team" but here the DAO took over during the launch time, so that naming wouldn't make sense). Lockup: 12 months since token deployment (launch), and then linear vesting over 18 months starting after the cliff.&#x20;

**Initial contributors 9.20%** (usually referred to as "investors" but here they were all forced to put a lot of time since more than half a year before launch, so that naming wouldn't make sense). Lockup: 12 months since token deployment (launch), and then linear vesting over 12 months starting after the cliff.

See their contributions and work over 2021 clearly here:

{% embed url="https://medium.com/gearbox-protocol/product-evolution-from-an-idea-to-an-app-0-to-1-contributors-united-832154e3c7ba" %}

### Company Wallet: 11.52%. Locked > 1 year + vesting.

**Company wallet** lockup: 12 months since token deployment (launch), and then linear vesting over 18 months starting after the cliff. Address: [0xa8b1d00b1d224e83760963e361b7f676581a622d](https://etherscan.io/address/0xa8b1d00b1d224e83760963e361b7f676581a622d)
