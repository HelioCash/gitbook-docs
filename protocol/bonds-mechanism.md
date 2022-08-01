# Bonds (HBOND)

![](<../.gitbook/assets/Bonds.png>)

### What are HBOND (Bonds)?

Bonds are unique tokens that can be utilized to help stabilize HELIO price around peg (4,000 HELIO = 1 ETH) by reducing the circulating supply of HELIO if the TWAP (time-weighted average price) goes below peg.

### When can I buy HBOND (Bonds)?

HBOND can be purchased only on contraction periods, when TWAP of HELIO is below 1.0. Every new epoch on contraction periods, HBONDs are issued in the amount of 3% of current HELIO circulating supply, with a max debt amount of 45%. 

This means that if bonds reach 45% of circulating supply of HELIO, no more bonds will be issued. 

{% hint style="info" %}
Note that during a zen epoch (when an epoch ends with a TWAP between 1.0 - 1.01), **no HBOND will be issued, even though the Boardroom does not print.**
{% endhint %}

{% hint style="danger" %}
HBOND TWAP (time-weighted average price) is based on the HELIO TWAP from the previous epoch as it ends. In other words, the HELIO TWAP is real-time but the HBOND TWAP is not.
{% endhint %}

### Where can I buy HBOND (Bonds)?

You can buy HBONDs if any are available through [helio.cash](https://helio.cash/bond) in the boardroom. Anyone can buy as many HBONDs as they want as long as they have enough HELIO to pay for them.

There is a limit of available HBONDs per epoch during contraction periods (3% of HELIO's current  circulating supply), and are sold first-come-first-serve.

### Why should I buy HBOND (Bonds)?

The first and most important reason to buy HBOND is that they help to maintain the peg, but they are not the only measure in place to keep the protocol on track.&#x20;

HBONDs don't have an expiration date, so you can view them as an investment in the long-term health of the protocol to be redeemed for a premium at a later date.

#### Incentives for Holding HBOND

The idea is to reward HBOND buyers for helping the protocol, while also protecting the protocol from being manipulated by big players.

So after you buy HBOND using HELIO , you have two possible ways to get your HELIO back:

1. Sell back your HBOND for HELIO **while the peg is between 1 - 1.1** (4,000 HELIO = 1 ETH) with no redemption bonus. This is in place to prevent an instant dump as soon as peg is recovered.
2. Sell back your HBOND for HELIO **while the peg is above 1.1** (4,000 HELIO = 1 ETH) with a bonus redemption rate.

The longer you hold, the more both the protocol and you benefit from HBOND.

{% hint style="success" %}
Example:

1. When HELIO = 0.8, burn 1 HELIO to get 1 HBOND (HBOND price = 0.8)
2. When HELIO = 1.15, redeem 1 HBOND to get 1.105 HELIO (HBOND price = 1.27)&#x20;
{% endhint %}

So, which one is better?

If I buy HELIO at 0.8, and hold it until 1.15 and then sell, I'm getting +$0.35 per HELIO .

But, if I buy HELIO at 0.8, burn it for HBOND, and redeem it at 1.15, I'm getting 1.105 HELIO \* 1.15 (HELIO current price) = 1,271 (+$0.47) per HBOND redeemed.

But, what if getting back to peg is taking too long?

We will adjust our use cases to have different behaviours on contraction and expansion periods to benefit both HELIO and HBOND holders when needed.

### What is the formula to calculate the redHELIOtion bonus for HBOND?

To encourage the redHELIOtion of HBOND for HELIO when HELIO 's TWAP > 1.1 and in order to incentivize users to redeem bonds at a higher price, HBOND redHELIOtion is designed to be more profitable with a higher HELIO TWAP value. The HBOND to HELIO ratio is 1:R, where R can be calculated using the formula as shown below:

$$
R=1+[(HELIO twapprice)-1)*coeff)]
$$

$$
coeff = 0.7
$$

### When can I swap HBOND for a premium?

You can only redeem HBONDs for a premium when the previous epoch's TWAP is greater than 1.1.
