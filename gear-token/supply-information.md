---
description: GEAR token contract and distribution information.
---

# Supply Information

GEAR token is an ERC20 utility token, starting as a governance token for the protocol - and then possibly taking any other new function the DAO could envision for it. The supply of GEAR is capped at 10,000,000,000 (10 billion) which can't be technically changed. See in source code.

Token contract ERC-20: [0xba3335588d9403515223f109edc4eb7269a9ab5d](https://etherscan.io/token/0xba3335588d9403515223f109edc4eb7269a9ab5d)\
Decimals: 18\
Symbol: $GEAR\
Coingecko: [https://www.coingecko.com/en/coins/gearbox](https://www.coingecko.com/en/coins/gearbox)

{% hint style="success" %}
Only \~3% of the total supply per year (from the DAO portion holding > 40%) goes into different initiatives & liquidity mining. The goal is to bring that number down as much as possible. All distributions beyond the initial can be found in [monthly-quarterly DAO reports](https://gearboxprotocol.notion.site/Monthly-Reports-6849871a9bae44dfb903531c0a997e8f). **There is no new inflation in GEAR:** only DAO grants and rewards for different activities: liquidity mining, stakers, and contributors. All at a relatively low rate.
{% endhint %}

#### Circulation Details

Most vestings started back in 2022 and have almost ended going into 2024. The DAO started with >55% and is currently at about 40% after multiple reward stages for users and DAO members. See details below. There are barely any vestings left for 2024 as they have almost fully unlocked in 2023. Nearly full circulation has been achieved, so there is no new overhang in the token supply.

You can consider circulating market cap to be \~50% of the entire 10B supply.

All the details, vesting contracts, and names are below.

***

## Initial Supply Information

GEAR supply has been split according to a many different contributor roles:

![Early community maintain majority of voting power. See governance page.](<../.gitbook/assets/Screen Shot 2021-12-10 at 18.26.31.png>)

### Community DAO Portion: \~58%. No vesting.

* **DAO Treasury Multisig**: originally 51.00%. Up to DAO to decide, managed by the DAO-enacted [treasury multisig](../governance/setup/guards-multisigs.md#financial-treasury-multisig-or-5-9). Address[: 0x7b065fcb0760df0cea8cfd144e08554f3cea73d1](https://etherscan.io/address/0x7b065fcb0760df0cea8cfd144e08554f3cea73d1).
  * Out of that, 2.766% to [DAO Round Part 1](https://snapshot.org/#/gearbox.eth/proposal/0x3e51eb2ced35e3ce61a83333f0a5cedf4cc7380e71a8f7a493d2e0f46073f85b). Lockup ends on July 15 of 2023, upon which 1 year of linear vesting will take place throughout 365 days, until July 2024.
  * Out of that, 1.057% to [DAO Round Part 2](https://snapshot.org/#/gearbox.eth/proposal/0xe10c53c3a1abb709ca724b8a9959c2afd84859397ec97956eb990b6538334137). Lockup ends on September 15 of 2023, upon which 1 year of linear vesting throughout 365 days, until September 2024.
* **Credit Account Mining**: 5%. Mined by 5,000 participants in the [ceremony](../overview/launch-phases/). No vesting.

{% content-ref url="../overview/launch-phases/credit-account-mining.md" %}
[credit-account-mining.md](../overview/launch-phases/credit-account-mining.md)
{% endcontent-ref %}

* **Community Testers**: \~1.085%. No vesting. _Originally, 1.267% were allocated, but community members performed onchain sleuthing and reduced this number._ [_Old distributor contract_](https://etherscan.io/address/0xadc72d5c034c189f5c0b03c7bac21ac50b9d01f1)_._&#x20;
* **Early Discord members**: \~0.348%. No vesting. _Originally, 0.476% were allocated, but after 9 months of claimants now showing up, the tokens were repurposed._ [_Old distributor contract_](https://etherscan.io/address/0xadc72d5c034c189f5c0b03c7bac21ac50b9d01f1)_._&#x20;

{% content-ref url="../overview/launch-phases/early-drop.md" %}
[early-drop.md](../overview/launch-phases/early-drop.md)
{% endcontent-ref %}

* **Retroactive rewards for 2021**: approximately 0.5% \[with 0.041% repurposed for other activities]. No vesting. As we set on to a few stages of the community distribution, we expected technical difficulties with some claimants. Instead, community members performed onchain sleuthing an a good portion of GEARs was saved. This was [decided to be used as a retroactive LP + CA GEAR reward](https://gov.gearbox.fi/t/gip-22-gearbox-v2-liquidity-mining-programs/1550) program. _This is from where the drop for testers and discord users happened, and remaining used for repurposed activities like retroactive drop._

{% hint style="info" %}
_Launch time_ is technically TGE, when the DAO was formed: December 15, 2021. If you read this in December 2023 & beyond, keep in mind that all seed vestings have ended.
{% endhint %}

### Initial external contributors: 1.28%. Locked > 1 year + vesting.

These are some amazing people who have contributed to the technical development but weren't committing capital, yet were incentivized to work further. Lockup: 12 months since token deployment (launch), and then linear vesting over 18 months. Ends in June 2024.

### Early backers: 9.20%. Locked > 1 year + vesting.

**Initial contributors 9.20%** (usually referred to as "investors" but here they were all forced to put a lot of time, so that naming wouldn't make sense - see at the bottom of the page for details). Lockup: 12 months since token deployment (launch), and then linear vesting over 12 months. Vesting ended already! See their contributions and work over 2021 clearly here:

{% embed url="https://medium.com/gearbox-protocol/product-evolution-from-an-idea-to-an-app-0-to-1-contributors-united-832154e3c7ba" %}

### Initial core contributors: 20%. Locked > 1 year + vesting.

**Initial core members 20%** (usually referred to as "team" but here the DAO took over during the launch time, so that naming wouldn't make sense). Lockup: 12 months since token deployment (launch), and then linear vesting over 18 months. Ends in June 2024.

### Initial company wallet: 11.52%. Locked > 1 year + vesting.

**Company wallet** lockup: 12 months since token deployment (launch), and then linear vesting over 18 months. Ends in June 2024. Address: [0xa8b1d00b1d224e83760963e361b7f676581a622d](https://etherscan.io/address/0xa8b1d00b1d224e83760963e361b7f676581a622d). This is outside of the scope of the DAO, and can be used for discretionary activities. This is a company that kickstarted the first protocol development pre-DAO launch. Not related to the DAO. _Keep in mind that some of those reserves were used to onboard new pre-DAO contributors, auditor engagements, external work performed before the DAO was established, etc._

{% hint style="info" %}
All of the vestings can be verified on-chain, no trust required. Community retains the largest portions both in terms of the distribution and in terms of voting weights.

**You can check those by going to the TokenDistributor contract**:

* check contributorsList \[3] to find yourself/someone;
* fill in your/eligible address from \[3] into \[2] contributorVestingContracts. That will give you the corresponding personal vesting contract for that address.
{% endhint %}

{% embed url="https://etherscan.io/address/0xf7512B2B20Cf427ADD8b01D8CDEef97a4B0E2C27#readContract" %}
[https://etherscan.io/address/0xf7512B2B20Cf427ADD8b01D8CDEef97a4B0E2C27#readContract](https://etherscan.io/address/0xf7512B2B20Cf427ADD8b01D8CDEef97a4B0E2C27#readContract)
{% endembed %}

## Early Backers and DAO Round 2022

<figure><img src="../.gitbook/assets/gearbox dao investors backers.jpg" alt=""><figcaption><p>The information on rounds, aka early contributors with vested GEAR, was taken from the main <a href="https://gearboxprotocol.notion.site/Gearbox-DAO-23966f122ae4421492819242b30a0e7a">Notion page</a>.</p></figcaption></figure>

* $1.585M DAO Round Part 2 in September 2022 at $150M valuation FDV with 1 year lockup and 1 year linear vesting after, ending in September 2024. [Read more here](https://snapshot.org/#/gearbox.eth/proposal/0xe10c53c3a1abb709ca724b8a9959c2afd84859397ec97956eb990b6538334137). _1.05% of supply._
* $4.15M DAO Round Part 1 in August 2022 at $150M valuation FDV with 1 year lockup and 1 year linear vesting after, ending in July 2024. [Read more here](https://medium.com/gearbox-protocol/dao-monthly-update-july-2022-4ce73c8fac6). The list of names: [Placeholder](https://twitter.com/placeholdervc?lang=en), [Zee Prime](https://twitter.com/ZeePrimeCap), [LedgerPrime](https://twitter.com/ledger\_prime), [Polymorphic](https://twitter.com/polymorphiccap) and [GCR](https://twitter.com/Globalcoinrsrch). See [Blockworks](https://blockworks.co/gearbox-shifts-into-v2-with-4m-funding-boost/) piece. _2.767% of supply._
* $2.3M pre-DAO Contributor Round in summer 2021. [Read here](https://medium.com/gearbox-protocol/product-evolution-from-an-idea-to-an-app-0-to-1-contributors-united-832154e3c7ba) how **these legends have actually helped Gearbox Protocol development**! The focus was on founders and angels who could help refine as well as push the product out there. [Variant Fund](https://twitter.com/variantfund), [1kx](https://twitter.com/1kxnetwork), [Lido Finance](https://twitter.com/LidoFinance) \[[P2P](https://twitter.com/P2Pvalidator)], [Focus Labs](https://twitter.com/fcslabs), [eGirl Capital](https://twitter.com/egirl\_capital), [Igor Barinov](https://twitter.com/barinov) of xDai ([zkBob](https://www.google.com/search?q=zkbob\&oq=zkbob\&aqs=chrome..69i57j69i59l2j69i60l2j69i61l2j69i60.771j0j7\&sourceid=chrome\&ie=UTF-8) & [Gnosis Chain](https://twitter.com/gnosischain)), Maker Mafia (ex & current MKR devs), [Stani Kulechov](https://twitter.com/StaniKulechov) of [Aave](https://twitter.com/AaveAave), [Anton](https://twitter.com/k06a) & [Sergey](https://twitter.com/deacix) of [1inch](https://twitter.com/1inch), [Cobie](https://twitter.com/cobie), [Launchub](https://twitter.com/LAUNCHub), [Fiskantes](https://twitter.com/Fiskantes) & [Zee Prime](https://twitter.com/zeeprimecap?lang=en), [Darren](https://twitter.com/Darrenlautf) & [Daryl](https://twitter.com/Daryllautk) Lau, [DegenScore](https://twitter.com/DegenScore), Sergey of [ICODrops](https://twitter.com/ICODrops), [Elias Simos](https://twitter.com/eliasimos) of [Rated](https://twitter.com/ratedw3b), [Santiago Santos](https://twitter.com/santiagoroel), [Larry Cermak](https://twitter.com/lawmaster) of [The Block](https://twitter.com/TheBlock\_\_), [Encode Club](https://twitter.com/encodeclub). _All lockups have ended in December 2023. 9.20% of supply._
