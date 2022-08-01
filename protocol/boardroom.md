# Boardroom

## The Boardroom User Interface

![The Boardroom user interface](<../.gitbook/assets/Boardroom.png>)

Let's take a look at each element of the Boardroom user interface and what it means.

1. **NEXT EPOCH**\
   The amount of time remaining until the next epoch.
2. **CURRENT EPOCH**\
   The number of the current epoch.
3. **HELIO PEG (TWAP)**\
   The TWAP (time-weighted average price) of the HELIO peg. The Boardroom only mints new HELIO as rewards for HSHARE stakers when this value **is above 1.01** **at the end of the current epoch**.
4. **APR**\
   The yield for HSHARE stakers in the Boardroom **if the Boardroom was printing every epoch**. This calculation is based on **the last recorded print in the Boardroom**.
5. **HSHARES STAKED**\
   ****The total amount of HSHARE currently staked in the Boardroom.
6. **HELIO Earned**\
   ****The amount of HELIO you've earned as rewards for staking HSHARE in the Boardroom.
7. **HSHARE Staked**\
   The amount of HSHARE you currently have staked in the Boardroom.

### Boardroom Specifications

* Epoch duration: 6 hours
* Any interaction with the boardroom will reset both timers. That's 3 epochs (18 hours) to withdraw your $HELIO rewards, and 6 epochs to unstake your $HSHARE (36 hours).**&#x20;
*   Distribution of HELIO during expansion (Boardoom printing):
    **80%** goes to Boardroom HSHARE stakers as rewards\
    **20%** goes to the Treasury
    **5%** goes to DAO fund
* Epoch Expansion: Current expansion cap base on HELIO supply, if there are bonds to be redeemed, 65% of minted HELIO goes to the Treasury until it's sufficiently full to meet bond redemption. If there is no debt, it will follow max capped expansion rate..

{% hint style="info" %}
Note that the Boardroom **does not** print any rewards for HSHARE stakers when the Boardroom TWAP < 1.01.
{% endhint %}

## Boardroom FAQ

### **1. Once HBONDs are issued, does the Boardroom stop printing HELIO until we are above peg again?**

Staking HSHARE will only give you HELIO rewards when the price of HELIO is above the peg (4,000 HELIO to 1 ETH), but not when it is under the peg.

### **2. What happens if I interact with the Boardroom in any way? Are there any lockup periods?**

Yes, there are two lockup timers. One for HELIO rewards and one for staked HSHARE. **Any interaction with the Boardroom will reset both timers.** The lockup period for withdrawing HELIO rewards is **3 epochs (18 hours)**, or **6 epochs (36 hours)** to unstake your HSHARE.

### **3. Are the Boardroom rewards pro-rated by time? For example, if I stake three hours before the end of an epoch versus five hours before the end of an epoch, would I get different rewards?**

No, Boardroom rewards are determined by how much you have staked at the time of printing (i.e., at the end of one epoch and the start of the other). It doesn't matter if you stake three hours before or thirty seconds before the emissions occur.

### 4. If I remove my HSHARE from the Boardroom without first collecting my HELIO , will they be lost forever?

No, they will still be there to collect whenever you need.

### 5. The Boardroom APR dropped because we're in a "debt phase." What does that mean?

A debt phase takes place during expansion epochs that start after a contraction period where there are still HBOND to be redeemed.

65% of expansion during a debt phase is allocated to the treasury fund to prepare for subsequent HBOND redemption down the road. This amount is always reserved, regardless of whether HBOND holders are redeeming bonds or not.

Once enough HELIO is sufficiently stocked in the treasury to satisfy the redemption of all circulating HBOND, expansion rates will resume to normal.

### 6. If we're in a debt phase, how long will it last until the Boardroom continues printing as normal?

The debt phase will last as long as is necessary to adequately pay back outstanding HBOND debt. Please keep in mind that the DAO will also need to collect a little extra, as there needs to be a cushion to cover the bonus premiums when people redeem HBOND over peg.\
\
There's no exact way of calculating how many epochs it will take, since the protocol doesn't know exactly when people will redeem their HBOND. The debt phase cannot end until the treasury has enough HELIO to cover the redemption of all outstanding HBONDs plus a premium.

### 7. At the end of the epoch, the Boardroom did not print HELIO, but then no HBOND(s) were issued either. Why?

There is a balanced state "at peg" when HELIO 's TWAP is between 1.00 and 1.01, which results in no contraction or expansion of the circulating supply of HELIO . This is referred to as a **zen epoch**.

### 8. If HELIO continues to climb above the price of the peg, will that influence how long the debt phase lasts?

Depending on the price of HELIO, the Boardroom print will have to adjust to provide a buffer for any unclaimed HBOND. As the price of HELIO climbs above the peg, more HELIO needs to be distributed to the treasury to account for HBOND redemption plus premiums.

### 9. How can I figure out what my future HELIO rewards will be from the Boardroom?

Let's take a look at a simplified example for a _non-debt phase_: say you have 1 HSHARE staked out of 10 total HSHAREs staked in the Boardroom. In this case, you will receive 10% of the total HELIO printed in the Boardroom.&#x20;

For this example we are assuming that there is a total circulating supply of 4,000 HELIO and the current expansion rate is at 4%, so a total of 400 HELIO will be printed in the Boardroom. Under the protocol's current rules, 75% of those newly printed HELIO will be distributed to HSHARE stakers in the Boardroom. (See the [HELIO Distribution](helio -distribution.md) page for more details on how HELIO is distributed within the protocol.)\
\
Therefore, you would get: ((0.04 _\*_ 10000) _\*_ 0.75) \* (1/10) = **30 HELIO **.\
\
Thus, the formula to calculate your rewards is as follows:\
((_ExpansionRate_ \* _CirculatingHELIO Supply)_ \* 0.75) \* (_YourHSHAREStake_ / _TotalHSHAREStaked_)

### 10. How long will it take for HSHARE to pay itself off from HELIO rewards based on current prices?

This will vary constantly as the APR in the Boardroom fluctuates, along with other variables such as the price of HELIO .

&#x20;For a quick estimation, however, you can do the following:

1. Take the total APR shown in the Boardroom and divide that by 365 to get the daily APR. (For this example we will say the daily APR is 5%.)
2. Multiply that daily APR by the current market price of the total HSHARE you have staked to see what your daily rewards are. (In this example, we have 5 HSHARE, each worth $500, for a total amount staked of $2500. Your daily return in this case would be $2500 \* 0.05, which comes out to $125 per day.)
3. Take your initial buy-in price for HSHARE and divide it by your daily rewards. If you bought these 5 HSHARE at a higher price, say $700 for example, in the current market conditions you would recover your initial investment of $3500 in 3500/125 or 28 days.
