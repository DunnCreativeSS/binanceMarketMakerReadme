# binanceMarketMakerReadme

This is the README for the Binance Market Maker repo, which has been made private. If you'd like access, just hit the 'sponsor' button near the top and follow the directions!



Lucky for me I already have a Binance futures market maker — and with a wee bit of edits to the code, it ran fine on margin 5x, too! I ran the futures on 100x and orders of 0.002 BTC and it won the futures contest in ~1hr.


Check g543 for the total. Woo!


I was +0.5% for most of my bot run on futures, ended at -1% on equity.


I was down about 21% — of my whopping $46 — on margin.


https://imgur.com/undefined


Win Binance trading competitions! I won my share of 10k BNB for futures trading and 40k BNB for spot/margin trading 1+ BTC in <3 hours in this recent Binance giveaway: https://www.binance.com/en/support/articles/360040070651


Setup:


1. Clone or download repo
2. cd into dir
3. python3 setup.py install


For our competition run, Coindex Labs is optimizing these input variables using our proprietary AI. Note that the defaults here will probably lose funds, they're not optimized or recommended.



binApi is your api key (futures enabled...)


binSecret is your api secret...


5. python3 market_maker.py
6. fun and profit!


https://hackernoon.com/porting-a-bot-to-binance-futures-market-making-competition-6v6a31qh


Track our bot's delta in real-time (after the test bot's run is complete) here: http://coindexbot.duckdns.org


Original README.md as follows:


Sample market maker bot
===

Strategy
---

The bot layers bids and offers around the market mid, which it attempts to calculate from the order book. The spread between quoted bids and offers is determined by a user-set risk charge on volatility. Volatility is estimated by an EWMA (Exponentially Weighted Moving Average Process) with frequency and parameters that may also be set by the user.

Set up
---

This bot requires python3 and the [Deribit api wrapper](https://pypi.org/project/deribit_api/).

To set up the bot, edit the `KEY` and `SECRET` variables in the code to your credentials. You can obtain those from the [Deribit account](https://www.deribit.com/main#/account?scrollTo=api).

To start the bot, run `python3 market_maker.py`.

Disclaimer
---

Different market conditions will produce different results. This code is for sample purposes only. It comes as is, with no warranty or guarantee of performance.
