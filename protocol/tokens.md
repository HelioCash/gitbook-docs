# Tokens

### HELIO - Helio.Cash Token

![helio.cash (HELIO )](<../.gitbook/assets/helio.png>)

Contract: [0xB38B969f151E8217C917fE0532382172BB6Fb83E](https://polygonscan.com/address/0xB38B969f151E8217C917fE0532382172BB6Fb83E)

The HELIO token is designed to be used as a medium of exchange. The built-in stability mechanisms within the protocol aim to maintain HELIO 's peg of 4,000 HELIO = 1 Ethereum (ETH) in the long run.&#x20;

{% hint style="warning" %}
Note that HELIO **actively pegs via an algorithm**, but that **does not mean** it will be valued at 4,000 HELIO to 1 ETH at all times as **it is not collateralized**. **HELIO is not to be confused for a crypto or fiat-backed stablecoin.**
{% endhint %}

### HSHARES - HELIO Shares

![HSHARE](<../.gitbook/assets/hshare.png>)

Contract: [0x8521F10339fA59417C90d3808426659b452a73E8](https://polygonscan.com/address/0x8521F10339fA59417C90d3808426659b452a73E8)

HELIO Shares (HSHARE) are one of the ways to measure the value of the Helio Cash Protocol and shareholder trust in its ability to consistently maintain HELIO close to peg. During epoch expansions the protocol mints HELIO and distributes it proportionally to all HSHARE holders who have staked their tokens in the [**Boardroom**](boardroom.md).

HSHARE has a **maximum total supply of 29,000** tokens distributed as follows:

1. _Treasury/DAO Allocation: 2,200_ HSHARE vested linearly 12 months\*
2. _Team Allocation: 2,000_ HSHARE vested linearly over 12 months
3. _Rewards: 23,000_ HSHARE are allocated for incentivizing liquidity providers in two farming pools for 12 months
4. Initial mint: 1000 HSHARE minted upon contract creation.

{% hint style="success" %}
The Helio Cash team will use the treasury funds in any way that they feel is best for the long-term success of the protocol.&#x20;
{% endhint %}

### [HBOND - HELIO Bonds](bonds-mechanism.md)

![HBOND](<../.gitbook/assets/hbond.png>)

Contract: [0x13Cc4910a82b7FB56Ee5e8e849dd314944114dDE](https://polygonscan.com/address/0x13Cc4910a82b7FB56Ee5e8e849dd314944114dDE)

The main purpose of HELIO Bonds (HBOND) is to help incentivize fluctuations in the HELIO supply during epoch contraction periods. When the TWAP (time-weighted average price) of HELIO falls below 4,000 to 1 ETH, HBONDs are issued and can be bought with HELIO at the current price. Exchanging HELIO for HBOND burns HELIO tokens, taking them out of circulation (deflation) and helps to get the price back up to peg. These HBOND can be redeemed for HELIO when the price is above peg in the future, plus a premium based on how high above peg we currently are. This conversely creates inflation and subsequent sell pressure for HELIO when it is above peg, helping to push it back toward 4,000 HELIO to 1 ETH ratio.

{% hint style="info" %}
Unlike early algorithmic protocols, HBONDs do not have expiration dates.
{% endhint %}

All HBOND holders will be able to redeem their HBOND for HELIO tokens as long as the treasury has a positive HELIO balance, which typically happens when the protocol is in epoch expansion periods.
