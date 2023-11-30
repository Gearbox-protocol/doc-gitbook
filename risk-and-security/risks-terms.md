---
description: Protocol and Interface risks every user must be aware of.
---

# Risks and T\&C

It is important to distinguish between an interface (application) that is operated by a normal web2 company - and the onchain protocol where all the logic is and that is not controlled by anyone. While the company can block its interface and prohibit its use, the protocol is fully in the hands of governance and is not managed by any single person or entity.&#x20;

{% hint style="success" %}
It's crucial for the DAO to find robust solutions and keep innovating, seeking to improve Gearbox security. You can find more information on such efforts in the [**Audits**](audits-bug-bounty.md) section.
{% endhint %}

Companies have their own legal disclaimers and risks associated, which you must go through and accept if you use the interface. **For instance, you must understand that an interface not being accessible can become an obstacle to you managing your position. But it doesn't mean that you cannot access your position or assets via smart contract directly or some other interface.**

{% hint style="danger" %}
This section is dedicated to explaining risks related to Gearbox Protocol on the contract level and conceptually. **We believe that outlining risks explicitly creates stronger accountability in the community and gives power back to the users of the protocol.** The risks presented below are general across many DeFi protocols. Ask more on [Discord](https://discord.gg/JssNVvxscK).
{% endhint %}

## **Protocol Technical Disclosure**

{% hint style="info" %}
Some of the disclosures can mimic interface-related concerns below.
{% endhint %}

#### Oracle Risk

In its current stage, Gearbox Protocol uses Chainlink Price Feeds. While the industry in general uses the same service, it is imperative to understand that oracles are a crucial point of DeFi infrastructure. An oracle going rogue or reporting incorrect data, may cause cascading liquidations or incorrect protocol operations. This can result in bad debt and loss of user funds.&#x20;

#### Sandwich attacks and MEV

No traders on Ethereum are safe from MEV attacks, and this is not something unique to Gearbox Protocol either. The DAO can find solutions and cooperate with protocols who provide MEV protection. Users should exercise trades with caution and watch out for their slippage. And for example, select better RPCs that protect you from being sandwhiched.

#### De-peg of base assets or stablecoin risks

It can happen that stablecoin issuers introduce boundaries as to who can use them, or freeze accounts. This can cause issues in the way protocols work, and Gearbox Protocol is no exception to that. In the ethos of decentralization, Gearbox DAO should strive to improve its collateral base to limit cases leading to possible bad debt accrual. However, the current version of Gearbox has isolated lending only, in which case the risk is contained within LP pools.

#### Liquidations and black-swan events

[Liquidations](../overview/liquidations/) do not depend on the protocol or any member involved. Liquidators are third-party workers open to anyone. It can happen that liquidators malfunction or do not perform, despite [economic incentives for liquidators](../overview/liquidations/) being in place. This can under-collateralize the protocol and make [LPs](../lending-market/pools-and-apy.md) lose their capital. To prevent that, DAO can implement token-backed backstops, increase[ Reserve Fund](../overview/liquidations/insurance-fund.md), onboard more professional liquidators, and so on.&#x20;

#### Risks of allowed tokens / contracts lists

[AllowedList](../overview/credit-account/#allowed-list-policy) defines where Gearbox Protocol users can deploy their leverage funds into. Wrong liquidation thresholds or hacks on the side of those assets can result in the insolvency of LP pools.&#x20;

#### Can't withdraw capital as LP due to the entire LP pool being in use

While the protocol can remain sane and over-collateralized, if the entire [LP](../lending-market/pools-and-apy.md) pool is borrowed, as an LP you would not be able to pull out your capital in that moment. This is the same scenario that Aave, Compound, or other protocols have in common and is pretty standard.

{% hint style="warning" %}
Usually, in DeFi protocols forced liquidation is not implemented. This can lead to cases of insufficient liquidity for a withdrawal operation. To mitigate this risk, the parameters for managing the interest rate curve of the pool are introduced (interest rate depends on utilization ratio of the pool). If the utilization of the pool stays too high, the Governance can further increase these parameters and thereby make lending more expensive. This will encourage borrowers to close loans and thereby make liquidity available.
{% endhint %}

#### Issues with wallets and signing transactions

Wallet connection and signing transactions on the user side can be an obstacle to interacting with the protocol, which must be taken into account.

#### Hacks and Software Issues

Taking advantage of the protocol in ways it is not intended to be, malfunction of the protocol which wasn't originally intended, and other security breaches which disrupt design of the systems. All of these issues can lead to partial or full loss of funds, which every user must understand and accept.

#### Governance and Multisig

Before governance transitions to full on-chain voting and execution, the execution of snapshot decisions or even on-chain events is still subject to multisig doing its job the right way.&#x20;

There is a timelock in place to prevent rogue multisig transactions. Moreover, multisig needs to make sure it operates well or its misalignment with the DAO [governance](../governance/setup/) can lead to users leaving the protocol. This is a model often used, but the risk should be understood nonetheless.

## **Interface Disclosure**

#### Gearbox App is in its Beta Stage

Gearbox App is in its beta stage, which means that the Gearbox App and all related software, including blockchain software and smart-contracts, are experimental. Gearbox App is provided on an “as is” and “as available” basis, without warranty of any kind, either expressed or implied, including, without limitation, warranties that the Gearbox App or any related software are free of defects, vulnerabilities, merchantable, fit for a particular purpose or non-infringing.&#x20;

#### Risk of Software Weaknesses

Although we make reasonable efforts to ensure that the Gearbox App and related software follow the high-security standards, we do not warrant or represent that the Gearbox App or any related software are secure or safe, or protected from fishing, malware or other malicious attacks. Further, the Gearbox App and related software may contain weaknesses, bugs, vulnerabilities, viruses or other defects which may have a material adverse effect on the operation thereof, or may lead to losses and damages for you, other users of Gearbox App, or third persons.

#### Risk Inherent in the Underlying Blockchain Networks

Gearbox App interacts with the Protocol deployed on the Ethereum Virtual Machine-compatible blockchain network(s) and more. As a result, any malfunction, breakdown or abandonment of such blockchain(s) may have a material adverse effect on the Gearbox App and Protocol.&#x20;

Moreover, advances in cryptography, or technical advances such as the development of quantum computing, could present risks to the Gearbox App and related blockchain software by rendering ineffective the cryptographic consensus mechanism that underpins the blockchain. The smart-contract concept, the underlying software and software platforms, including the blockchain networks, are still in an early development stage and unproven. Although it is very unlikely, the blockchain, as well as any other blockchain, can be attacked which may result in downtime, consensus split, long reorganization of the chain, 51 percent attack, or other adverse outcomes each of which may lead to complete loss of your assets implemented on such blockchain network.

#### Risk Inherent in the Protocol

Gearbox App interacts with the Protocol and when using the Gearbox App you may be exposed to certain risks related to the operation and functioning of the Protocol. The Protocol is complex, the majority of its components and functional elements are risky and experimental. You should not use or interact with the Protocol unless you fully understand how it works and the consequences of transactions carried out with the use of the Protocol. Gearbox App derives information from the Protocol, related software and underlying blockchain network(s) in an automated manner, which means that such information is not verified. As a result, such information may not be true, complete, timely, accurate, or sufficient.&#x20;

Furthermore, certain functions within the Protocol may be executed by third parties that may not act in a timely or reliable manner, or as expected or intended, or may fail to act, which can lead to partial or complete loss of your digital assets. That is related to untimely or imperfect [liquidations](../overview/liquidations/).

#### Risk of Flawed Logic of Gearbox App&#x20;

The underlying logic of the Gearbox App and related software may be flawed, defective or impaired, which can result in smart-contracts operating incorrectly or not as expected, or transactions being executed in violation of logic which underpins the smart-contracts, which can lead to partial or complete loss of digital assets used in the transaction.

#### Risk of Confusing User Interface

Certain user interface elements or design decisions of the Gearbox App can be confusing or mislead you, which may result in the execution of a different action or transaction than intended or desired, or connection of a wrong digital wallet, account or network.

#### Risk of Legal Uncertainty

Just like any other business, the intended activities of Gearbox may be subject to various laws and regulations in the countries where it operates or intends to operate. We might be obliged to obtain different licenses or other permissive documents in some or all jurisdictions where we intend to operate our business, therefore, our business in such jurisdictions shall always be subject to obtaining such licenses or permissive documents, if so directed by applicable laws. Furthermore, regulatory actions, orders or inquiries may adversely affect the Gearbox App and Gearbox, or impair our ability to make the Gearbox App available. Additionally, changes in applicable laws or regulations or evolving interpretations of existing law could, in certain circumstances, result in increased compliance costs or capital expenditures, which could affect our ability to carry on the business model and develop the Gearbox App and related software.

#### Risk of Theft

We make a commercially reasonable effort to ensure that any transactions carried out via the Gearbox App are secure. Notwithstanding the aforesaid, there is no assurance that there will be no theft of the digital assets as a result of hacks, sophisticated cyber-attacks, distributed denials of service or errors, double-spent attacks, flash-loan attacks, vulnerabilities or defects of the Gearbox App or related software, the Ethereum blockchain network or any other blockchain network, or otherwise. Such events may include, for example, flaws in programming or source code leading to exploitation or abuse thereof. Any of the above may lead to partial or complete theft or loss of digital assets used in transactions carried out through the Gearbox App or with the use of related software.&#x20;
