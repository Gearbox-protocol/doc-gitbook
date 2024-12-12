---
description: Staking and utility sinks that exist for GEAR.
---

# Utility & Staking

GEAR token is an ERC20 utility token. It started as a governance token for the protocol - and then could take any other new function the DAO could envision for it. [Supply information is here](supply-information.md).

GEAR is a functional multi-utility token which will be used as the native governance token and economic incentives which will be distributed to encourage users to exert efforts towards contribution and participation in the ecosystem on the Gearbox Protocol, thereby creating a mutually beneficial system where every participant is fairly compensated for its efforts. GEAR is an integral and indispensable part of the Gearbox Protocol, because without GEAR, there would be no incentive for users to expend resources to participate in activities or provide services for the benefit of the ecosystem. Given that additional GEAR will be awarded to a user based only on its actual usage, activity and efforts made on the Gearbox Protocol and/or proportionate to the frequency and volume of transactions, users of the Gearbox Protocol and/or holders of GEAR which did not actively participate will not receive any GEAR incentives.

Tokenomics can be adjusted in different ways. What is crucial is that the protocol has had the fee switch turned on by the DAO back in 2022, check what [fee streams it currently has](../overview/protocol-fees.md). There are 4 fee streams, and they are all configurable to adjust to different use cases and integrations. Vote!  It is important to note that holders of GEAR will not passively accrue rewards/fees just by holding tokens – they need to actively engage in various activities, e.g. staking, governance, provision liquidity to pools.

It is important to reiterate that smart contract protocols and pools such as the Gearbox Protocol simply comprise a set of autonomous blockchain-based smart contracts deployed on the relevant blockchain network, operated directly by users calling functions on it (which allows them to interact with other users and/or engage in trading or other activities in a multi-party peer-to-peer manner). There is no further control by or interaction with the original entity which had deployed the smart contract, which entity solely functions as a provider of technical tools for users, and is not offering any sort of securities product or regulated service nor does it hold any user assets on custody. As such, any token or other rewards which users potentially may earn from the protocol arise solely out of the user's involvement in the protocol by taking on the risk of interacting with other users and/or providing liquidity, and charging a fee for this work (e.g., trading fees, liquidity provider fees).



***

### 1. Main DAO Governance: Snapshot

GEAR allows users to propose and vote on overall protocol direction and protocol parameters, for example setting rates and incentive levels for different activities, onboarding supported assets and protocols, directing protocol treasury and grants to expand available utilities and to build out the ecosystem, with voting power based on staked GEAR tokens. That happens on snapshot, see how on [governance page](../governance/setup/). You can vote on proposals or propose yourself even if you don't hold idle GEAR but have them in the GEAR-ETH Curve LP. Then your GEAR is taken into account, for [delegation](../governance/setup/community-delegates.md) as well. Snapshot can expand its "strategies" to also account for [Quotas & Gauges](utility-and-staking.md#quotas-and-gauges) balances of stakers, and so on. It's configurable.

After governance launch there will be no individual or corporate entity or other active promoter, sponsor, or group or affiliated party that maintains sole control over the Gearbox Protocol.

It is the community members which would maintain and drive development of the Gearbox Protocol, so GEAR incentives would need to be distributed to promote enthusiasm for development efforts, community governance, and/or to increase community activity, in order to compensate users for their time, expertise and effort. Only users who have participated in submission of proposals, commenting, reviewing and/or voting will be entitled to receive GEAR token governance rewards.

{% content-ref url="../governance/setup/" %}
[setup](../governance/setup/)
{% endcontent-ref %}

### 2. Quotas and Gauges

GEAR stakers can freeze their tokens for 4 epochs (28 days) and vote on the extra rates borrowers are paying for every different asset. This is a very important protocol function, because it (1) creates better and more fair rate markets whereas (2) this extra fee is split between lenders to compensate them for their liquidity as well as the DAO (the fee goes into the [separate fee multisig](../governance/setup/guards-multisigs.md#fee-temporary-guard-5-10)).&#x20;

{% content-ref url="../governance/quotas-and-gauges/" %}
[quotas-and-gauges](../governance/quotas-and-gauges/)
{% endcontent-ref %}

### 3. GEAR-ETH Curve Pool

Gear Protocol itself does not provide any resources for utilisation, so liquidity providers would need to be incentivised to deposit assets into the liquidity pool for utilisation by borrowers. To compensate them for opportunity costs, the protocol would issue GEAR rewards to these users as a reward for their contributions (i.e. "liquidity mining").&#x20;

To encourage borrowers to utilise the protocol, GEAR rewards would also be distributed to reward these users which promote ecosystem adoption.

There is liquidity mining ongoing for the[ GEAR-ETH pair on Curve V2](https://curve.fi/#/ethereum/pools/factory-crypto-192/deposit). You take some impermanent loss on it potentially, but get an APR at the rate that might compensate for that and above. The rewards in GEAR accrued you need to claim yourself automatically, or go to Convex / Yearn for this.

Make sure to "Deposit & Stake" your Curve LP tokens, as their interface suggests.

<figure><img src="../.gitbook/assets/GEAR token Curve.png" alt=""><figcaption><p><a href="https://curve.fi/#/ethereum/pools/factory-crypto-192/deposit">https://curve.fi/#/ethereum/pools/factory-crypto-192/deposit</a></p></figcaption></figure>

{% hint style="success" %}
It is logical to expect that some of these utilities and staking contracts should be harmonized, so holders could do a few things at a time. Should it be? How? Should the LM move over from Curve to Uniswap? [Discuss these ideas and propose your solution](https://discord.com/channels/841203475606011905/1177177691842166844).
{% endhint %}

#### Others

There could be anyone offering utility sinks for GEAR. It's up to every holder individually to decide which of the utility sinks they want to engage in. Based on market developments, which fundamentally serve to promote certain aspects of the protocol. You can also propose and / or make your own staking contract, or propose to the DAO to offer something else. [Jump in Discord](https://discord.gg/gearbox) to discuss!
