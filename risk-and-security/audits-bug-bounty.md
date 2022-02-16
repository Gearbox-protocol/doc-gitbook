---
description: Reports on Gearbox Protocol security.
---

# Audits & Bug Bounty

{% hint style="warning" %}
Keep in mind that no number of audits can guarantee full safety. There are always high risks involved in DeFi, as many platforms are composable and depend on each other. There is no guaranteed return on Gearbox - you must [**understand the risks involved**](risks-terms.md).
{% endhint %}

## Audits

* **Consensys** Diligence Fuzzing (04/10/2021- 13/12/2021): [report](https://github.com/Gearbox-protocol/gearbox-contracts/blob/master/audits/ConsensysDiligence%20\_Fuzzing\_report.pdf)
* **ChainSecurity** (31/08/2021–13/12/2021): [report](https://github.com/Gearbox-protocol/gearbox-contracts/blob/master/audits/ChainSecurity\_Gearbox\_audit.pdf)
* **MixBytes** (06/07/2021–22/12/2021): [report](https://github.com/Gearbox-protocol/gearbox-contracts/blob/master/audits/MixBytes\_security\_audit\_report.pdf)
* Peckshield (22/07/2021 - 10/08/2021): [report](https://github.com/Gearbox-protocol/gearbox-contracts/blob/master/audits/Peckshield-10.08.2021.pdf)
* Peckshield (09/04/2021 - 03/05/2021): [report](https://github.com/Gearbox-protocol/gearbox-contracts/blob/master/audits/Peckshield-03.05.2021.pdf)

## Bug Bounty

Join the Bug Bounty with Immunefi! Help Gearbox stay safe and be rewarded for it.

{% embed url="https://immunefi.com/bounty/gearbox" %}

![https://immunefi.com/bounty/gearbox/](<../.gitbook/assets/Screenshot 2022-02-08 at 17.37.31.png>)

### Scope&#x20;

The scope of the bug bounty refers to the core contracts available at this repository: [https://github.com/Gearbox-protocol/gearbox-contracts](https://github.com/Gearbox-protocol/gearbox-contracts). _If you have found a bug that you think is within the security interests of the protocol but is outside of the scope of the repository above, please do notify us then anyway. We can decide ad-hoc together with you._

If you need more information on the protocol, please check:&#x20;

* Regular protocol documentation: [https://docs.gearbox.finance/ ](https://docs.gearbox.finance)
* Developer docs in progress: [https://dev.gearbox.fi/](https://dev.gearbox.fi)

**NOTE**: for bugs related to the interface which are just referring to typos and non-security related issues, please feel free to report them in a community [Discord](https://discord.gg/5YuHH9tvms) pro bono - and Gearbox community can maybe send nice GIFs your way. In case a bug you found is related to the interface and is outside of the scope, but has serious security concerns, please do report it as well and a bounty can be also decided ad-hoc. Again, you can ask all your questions in [Discord](https://discord.gg/JZgvmaenwn).

### Rewards&#x20;

Rewards are distributed according to the impact of the vulnerability. The final decision on the payout amount will be determined by the Gearbox DAO at its discretion.

| Severity  | Payment in USDC / other stablecoin |   |
| --------- | ---------------------------------- | - |
| Low       | Up to $5’000                       |   |
| Medium    | Up to $10’000                      |   |
| High      | Up to $25’000                      |   |
| Very High | Up to $75’000                      |   |
| Critical  | Up to $150’000 + GEAR              |   |

### Rules

{% hint style="info" %}
Determinations of eligibility, score and all terms related to an award are at the sole and final discretion of Gearbox Protocol working DAO members. The goal is to make sure the ecosystem is safe, and that proper bug bounty work is rewarded well.
{% endhint %}

In order to be considered for a reward, all bug reports must contain the following:&#x20;

* Description of suspected vulnerability&#x20;
* Steps to reproduce the issue so we can check it&#x20;
* Your name and/or colleagues if you wish to be later recognized&#x20;
* (Optional) A patch and/or suggestions to resolve the vulnerability

The following activities are prohibited by bug bounty program:&#x20;

* Any testing with mainnet or public testnet contracts: all testing should be done on private testnets
* Any testing with pricing oracles or third party smart contracts&#x20;
* Attempting phishing or other social engineering attacks against our employees and/or customers&#x20;
* Any testing with third party systems and applications (e.g. browser extensions) as well as websites (e.g. SSO providers, advertising networks)&#x20;
* Any denial of service attacks&#x20;
* Automated testing of services that generates significant amounts of traffic&#x20;
* Public disclosure of an unpatched vulnerability in an embargoed bounty

{% hint style="success" %}
Security is a continuous effort which must always be following protocol growth. As a DAO, it is imperative to constantly dedicate ample resources to ensure safety of user funds.
{% endhint %}
