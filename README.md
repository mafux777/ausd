# Ad-Hoc Analysis of Token Transfers related to events.

If you are just tuning in, here is what we know....
Acala provisioned the iBTC/aUSD LP with a configuration error meaning that too many rewards were being paid out. (Factor?)
People who noticed reinvested (compounding interest can be very powerful!)

People who had "enough" and wanted to take some profits:

1. Sold aUSD for other coins on Acala (e.g. IBTC, DOT, etc.)

2.Bridged aUSD over to Moonbeam and went on a shopping spree, driving the price of iBTC up to 80k$ (in GLMR) 

In the process, aUSD dropped to as low as 0.05$. It is currently at .70$ on Stellaswap, signifying that people expect a 30% "haircut" to cover losses
There are only about 5m xcAUSD on Moonbeam, only a fraction of all the aUSD which was minted this morning (UTC time): 3bn
The most interesting address on acala are these ones, since they show the big transfers (summed) of AUSD

Central player seems to be: https://sub.id/26JmEcghNmggvT46sojckg34Py9zFRKkCcFy3gr49hrFgT2k

Comments from Interlay:

- Between the pool going live on 2022-08-13 22:41:48 (+UTC) and 2022-08-14 16:00:00 (UTC), a total of 3.6 iBTC were bridged from Acala to Interlay
- A naive analysis shows that of the 3 accounts that bridged iBTC from Acala also redeemed iBTC for BTC
- A total of 3.3 BTC were redeemed from iBTC from accounts that used the same account id for the xcm transfer form Acala and requesting the redeem
- We have two independent tools used for analysis. Both open source and happy to share links if you need it
- Rolling back state on our chain will not be possible due to BTC being redeemed during the time of the issue as we can't update the Bitcoin chain state
- Damage to Interlay users seem to be contained to the iBTC/aUSD and to a smaller degree iBTC/GLMR pools
- Further investigation is necessary since accounts can transfer with each other and we haadn't had a chance yet to also take the StellaSwap/Moonbeam accounts into full consideration from our side

