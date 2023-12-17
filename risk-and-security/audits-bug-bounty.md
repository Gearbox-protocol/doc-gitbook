---
description: Reports on Gearbox Protocol security.
---

# Audits & Bug Bounty

{% hint style="warning" %}
Keep in mind that no number of audits can guarantee full safety. There are always high risks involved in DeFi, as many platforms are composable and depend on each other. There is no guaranteed return on Gearbox - you must [**understand the risks involved**](risks-terms.md).
{% endhint %}

## Audits

<figure><img src="../.gitbook/assets/Gearbox Protocol GEAR audits ABDK Chain Security Sigma Prime MixBytes (1).PNG" alt=""><figcaption></figcaption></figure>

* **ChainSecurity** (Q2-Q4 2023): full V3 coverage, [reports](https://github.com/Gearbox-protocol/security/tree/main/audits) (see multiple files)
* **ABDK** (Q2-Q4 2023): full V3 coverage, [reports](https://github.com/Gearbox-protocol/security/tree/main/audits) (see multiple files)
* **Decurity** (08/11/2023 - 20/11/2023): governor audit, [report](https://github.com/Gearbox-protocol/security/blob/main/audits/2023%20Dec%20-%20Decurity\_Governor\_Report.pdf)

Previous versions, including audits of many of the V3 contracts:

* **ChainSecurity** (23/02/2022 - 19/10/2022): full V2 coverage, [report](https://github.com/Gearbox-protocol/security/blob/main/audits/2022%20Oct%20-%20ChainSecurity%20report.pdf)
* **Consensys Diligence** (25/07/2022 - 12/08/2022): full V2 coverage, [report](https://github.com/Gearbox-protocol/security/blob/main/audits/2022%20Sep%20-%20Consensys%20Diligence.pdf)
* **Sigma Prime** (21/02/2022 - 06/08/2022): partial V2 coverage, [report](https://github.com/Gearbox-protocol/security/blob/main/audits/2022%20Aug%20-%20SigmaPrime\_Gearbox\_Smart\_Contract\_Security\_Assessment\_Report\_v2.pdf)
* **Consensys** **Diligence** Fuzzing (04/10/2021 - 13/12/2021): V1 coverage, [report](https://github.com/Gearbox-protocol/security/blob/main/audits/2021%20Dec%20-%20ConsensysDiligence%20\_Fuzzing\_report.pdf)
* **ChainSecurity** (31/08/2021 - 13/12/2021): V1 coverage, [report](https://github.com/Gearbox-protocol/security/blob/main/audits/2021%20Dec%20-%20ChainSecurity\_Gearbox\_audit.pdf)
* **MixBytes** (06/07/2021 - 22/12/2021): V1 coverage, [report](https://github.com/Gearbox-protocol/security/blob/main/audits/2021%20Dec%20-%20MixBytes\_security\_audit\_report.pdf)
* **Peckshield** (22/07/2021 - 10/08/2021): initial version coverage, [report](https://github.com/Gearbox-protocol/security/blob/main/audits/2021%20Sep%20-%20Peckshield-10.08.2021.pdf)
* Peckshield (09/04/2021 - 03/05/2021): first iteration coverage, [report](https://github.com/Gearbox-protocol/security/blob/main/audits/2021%20May%20-%20Peckshield-03.05.2021.pdf)

{% hint style="info" %}
Since Gearbox Protocol is modular, full protocol re-deployment is not required during changes. If approved by [governance](../governance/setup/), enacted [multisig](../governance/setup/guards-multisigs.md#technical-multisig-or-6-10) can take pieces in-and-out.
{% endhint %}

## Bug Bounty

Join the Bug Bounty with Immunefi! Help Gearbox stay safe and be rewarded for it.

{% embed url="https://immunefi.com/bounty/gearbox" %}

<figure><img src="../.gitbook/assets/Screenshot 2022-10-28 at 14.59.10.png" alt=""><figcaption><p><a href="https://immunefi.com/bounty/gearbox/">https://immunefi.com/bounty/gearbox/</a></p></figcaption></figure>

### Scope&#x20;

The scope of the bug bounty refers to the core contracts available in these repositories:

1. [https://github.com/Gearbox-protocol/core-v3](https://github.com/Gearbox-protocol/core-v3)
2. [https://github.com/Gearbox-protocol/integrations-v3](https://github.com/Gearbox-protocol/integrations-v3)
3. [https://github.com/Gearbox-protocol/oracles-v3](https://github.com/Gearbox-protocol/oracles-v3)
4. [https://github.com/Gearbox-protocol/governance](https://github.com/Gearbox-protocol/governance)&#x20;

{% hint style="success" %}
If you have found a bug that you think is within the security interests of the protocol but is outside of the scope of the repository above, please do notify us then anyway. We can decide ad-hoc together with you. 1/1 payouts has been done before based on this.
{% endhint %}

If you need more information on the protocol, please check:&#x20;

* Regular protocol docs: [https://docs.gearbox.finance/ ](https://docs.gearbox.finance/)
* Developer docs: [https://dev.gearbox.fi/](https://dev.gearbox.fi/)

**NOTE**: for bugs related to the interface which are just referring to typos and non-security related issues, please feel free to report them in a community [Discord](https://discord.gg/5YuHH9tvms) pro bono - and Gearbox community can maybe send nice GIFs your way. In case a bug you found is related to the interface and is outside of the scope, but has serious security concerns, please do report it as well and a bounty can be also decided ad-hoc. Again, you can ask all your questions in [Discord](https://discord.gg/JZgvmaenwn).

### Rewards&#x20;

Rewards are distributed according to the impact of the vulnerability. The final decision on the payout amount will be determined by the Gearbox DAO at its discretion.

<table><thead><tr><th>Severity</th><th>Payment in USDC / other stablecoin</th><th data-hidden></th></tr></thead><tbody><tr><td>Low</td><td>Up to $6,500</td><td></td></tr><tr><td>Medium</td><td>Up to $13,000</td><td></td></tr><tr><td>High</td><td>Up to $65,000</td><td></td></tr><tr><td>Critical</td><td>Up to $200,000 (+ GEAR)</td><td></td></tr></tbody></table>

### Disclosures and Multisig Actions

As a report for transparency on the actions of the multisig, as well as the disclosures related to certain actions, you can keep an eye on this transparency tool which details all that's going on:&#x20;

{% embed url="https://risk.gearbox.foundation/updates" %}

More info can also be found on GitHub:&#x20;

{% embed url="https://github.com/Gearbox-protocol/secutiry/tree/main/disclosures" %}

### Rules

{% hint style="info" %}
Determinations of eligibility, score and all terms related to an award are at the sole and final discretion of Gearbox Protocol working DAO members. The goal is to make sure the ecosystem is safe, and that proper bug bounty work is rewarded well.
{% endhint %}

In order to be considered for a reward, all bug reports must contain the following:&#x20;

* Description of suspected vulnerability&#x20;
* Steps to reproduce the issue so we can check it&#x20;
* Your name and/or colleagues if you wish to be later recognized&#x20;
* (Optional) A patch and/or suggestions to resolve the vulnerability

The following activities are **prohibited** by bug bounty program:&#x20;

* Testing with mainnet or public testnet contracts: all testing should be done on private testnets
* Any testing with pricing oracles or third party smart contracts&#x20;
* Attempting phishing or other social engineering attacks against our employees and/or customers&#x20;
* Any testing with third party systems and applications (e.g. browser extensions) as well as websites (e.g. SSO providers, advertising networks)&#x20;
* Any denial of service attacks&#x20;
* Automated testing of services that generates significant amounts of traffic&#x20;
* Public disclosure of an unpatched vulnerability in an embargoed bounty

{% hint style="success" %}
Security is a continuous effort which must always be following protocol growth. As a DAO, it is imperative to constantly dedicate ample resources to ensure safety of funds.
{% endhint %}
