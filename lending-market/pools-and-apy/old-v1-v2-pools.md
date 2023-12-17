# OLD: V1-V2 Pools

{% hint style="danger" %}
This page refers to the information about old V1-V2.1 pools.
{% endhint %}

{% content-ref url="../manage-liquidity.md" %}
[manage-liquidity.md](../manage-liquidity.md)
{% endcontent-ref %}

The pools below are the old V1-V2.1 ones.

<table><thead><tr><th width="170.78357926598557">Asset</th><th>Contract Address</th></tr></thead><tbody><tr><td>ETH (<a href="../../overview/faq.md#why-cant-i-trade-eth-on-dexes-via-wallet-connect">WETH</a>)</td><td><a href="https://etherscan.io/address/0xB03670c20F87f2169A7c4eBE35746007e9575901">0xB03670c20F87f2169A7c4eBE35746007e9575901</a></td></tr><tr><td>wstETH</td><td><a href="https://etherscan.io/address/0xB8cf3Ed326bB0E51454361Fb37E9E8df6DC5C286">0xB8cf3Ed326bB0E51454361Fb37E9E8df6DC5C286</a></td></tr><tr><td>USDC</td><td><a href="https://etherscan.io/address/0x86130bDD69143D8a4E5fc50bf4323D48049E98E4">0x86130bDD69143D8a4E5fc50bf4323D48049E98E4</a></td></tr><tr><td>DAI</td><td><a href="https://etherscan.io/address/0x24946bCbBd028D5ABb62ad9B635EB1b1a67AF668">0x24946bCbBd028D5ABb62ad9B635EB1b1a67AF668</a></td></tr><tr><td>FRAX</td><td><a href="https://etherscan.io/address/0x79012c8d491dcf3a30db20d1f449b14caf01da6c">0x79012c8d491dcf3a30db20d1f449b14caf01da6c</a></td></tr><tr><td>WBTC</td><td><a href="https://etherscan.io/address/0xB2A015c71c17bCAC6af36645DEad8c572bA08A08">0xB2A015c71c17bCAC6af36645DEad8c572bA08A08</a></td></tr></tbody></table>

## How was APY calculated in V1-V2.1?

Capital is required for traders and farmers to get leverage for their financial operations. For this, there are Liquidity Pools: anyone can become a liquidity provider by supplying assets in the Liquidity Pool. The profitability of LPs depends on the pool utilization ratio _U_ - the higher utilization, the higher interest rate. See a bit more on the [protocol-fees.md](../../overview/protocol-fees.md "mention") page.

Borrow APY is calculated according to formula

$$
r(t) = 
    \begin{cases}
        r_0 + \frac{U(t)}{U_1}\left(r_1-r_0\right), & U(t) \le U_1\\
        r_1 + \left(U(t)-U_2\right)\frac{r_2-r_1}{U_2-U_1}, & U(t) \in (U_1,U_2].\\
        r_2 + \left(U(t)-U_2\right)\frac{r_3-r_2}{1-U_2}, & U(t) > U_2.\\
    \end{cases}
$$

<table><thead><tr><th width="167">Asset pool</th><th width="82">r_0</th><th width="80">r_1</th><th width="91">r_2</th><th width="83" data-type="number">r_3</th><th width="90">U_1</th><th>U_2</th></tr></thead><tbody><tr><td>USDC</td><td>0</td><td>1</td><td>1.25</td><td>100</td><td>70</td><td>90</td></tr><tr><td>DAI</td><td>0</td><td>1</td><td>1.25</td><td>100</td><td>70</td><td>90</td></tr><tr><td>FRAX</td><td>0</td><td>1</td><td>1.25</td><td>100</td><td>70</td><td>90</td></tr><tr><td>wstETH</td><td>0</td><td>2</td><td>2.5</td><td>60</td><td>70</td><td>90</td></tr><tr><td>ETH</td><td>0</td><td>2</td><td>2.5</td><td>60</td><td>70</td><td>90</td></tr><tr><td>WBTC</td><td>0</td><td>2</td><td>2.5</td><td>60</td><td>70</td><td>90</td></tr></tbody></table>

[**Latest update 2**](https://snapshot.org/#/gearbox.eth/proposal/0x78615ba387512748a189cfdc39f1d3a7e835d1ce151b53049e42eff411fbee73): governance updated interest rate curve to two-point model.&#x20;

[**Latest update**](https://gov.gearbox.fi/t/gip-20-update-fees-interest-rate-curves/1571): governance voting to change pool interest rate curve parameters and make the curve more flat as a bootstrap mechanism for V2 Leverage Ninja launch. See the [logic](https://gov.gearbox.fi/t/gip-20-update-fees-interest-rate-curves/1571).

### V2-V2.1 Pool Caps

<table><thead><tr><th width="150">Asset</th><th width="113">Pool max</th><th width="150">Min pers borrow</th><th width="306">Max pers borrow</th></tr></thead><tbody><tr><td>USDC</td><td>N/A</td><td>60,000 USDC</td><td>1,000,000 USDC</td></tr><tr><td>DAI</td><td>N/A</td><td>60,000 DAI</td><td>1,000,000 DAI</td></tr><tr><td>FRAX</td><td>N/A</td><td>100,000 FRAX</td><td>1,000,000 FRAX</td></tr><tr><td>wstETH</td><td>N/A</td><td>75 wstETH</td><td>600 wstETH</td></tr><tr><td>WETH</td><td>N/A</td><td>30 WETH</td><td>600 WETH</td></tr><tr><td>WBTC</td><td>N/A</td><td>2 WBTC</td><td>50 WBTC</td></tr></tbody></table>

[**Latest update**](https://gov.gearbox.fi/t/gip-20-update-fees-interest-rate-curves/1571)**:** pool limits are effectively lifted. Any actual caps are just required by the architecture to have \*some\* number and can be lifted without a vote if the TVL approaches them. As for the min-max personal borrow limits, they have been established by another vote: [GIP-21](https://gov.gearbox.fi/t/gip-21-leverage-ninja-mode-limits-for-v2/1572), then [GIP-71](https://snapshot.org/#/gearbox.eth/proposal/0x6b01ac9fb32ef8004273592a62393ad24db810a0016a62e6ab6498a9c292bdbe).
