# Week 2 Notes
## Gambling Basics
### Gambling and Betting Markets
Gambling is usually defined as "a game of chance that involves monetary value".  There are typically 3 types of markets in which betting takes place:

1. Pari-mutuel
2. Bookmaking
3. Betting exchanges

#### Pari-Mutuel Betting
The fundamental idea is that everyone who bets (the **punters**) puts their money into a pool, and those who bet on the winner share out the pool in proportion to their bet.  This is the most popular form of gambling in horse racing and is probably the simpliest way to view the gambling market.

An example of pari-mutuel betting could include a two-horse race with White Queen and Red Queen and the gamblers place their bets as follows:

| Punter | White Queen | Red Queen | All Bets |
| :-- | --- | --- | --- |
| A | 10 | | 10 |
| B | 50 | | 50 |
| C | 100 | | 100 |
| D | | 30 | 30 |
| E | | 60 | 60 |
| **Total** | **160** | **90** | **250** |

The percentages of punters that bet on a particular horse would be reflected as the **probability** of that horse to win the race (i.e. White Queen received 160/250 bets therefore their probability is 64% to win the race).  Let's look at the **winnings**, **losses**, and **rate of return** under pari-mutuel betting.

| Punter | White Queen | Red Queen | All Bets | Share of Pot if White wins | Share of Pot if Red Wins | Win if White Wins | Win if Red Wins | RoR on Bet if White Wins | RoR on Bet if Red Wins | RoR Weighted By Probability |
| :-- | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| A | 10 | | 10 | 6% | 0% | 15.63 | 0 | 56% | -100% | 0% |
| B | 50 | | 50 | 31% | 0% | 78.13 | 0 | 56% | -100% | 0% |
| C | 100 | | 100 | 63% | 0% | 156.25 | 0 | 56% | -100% | 0% |
| D | | 30 | 30 | 0% | 33% | 0 | 83.33 | -100% | 178% | 0% |
| E | | 60 | 60 | 0% | 67% | 0 | 166.67 | -100% | 178% | 0% |
| **Total** | **160** | **90** | **250** | **100%** | **100%** | **250** | **250** |

- **Share of Pot**: for winners, the share of the payout is proportional to your share of bets on the winner
- **Winnings**: equal to your share of the pot times the pot (250 in this example)
- **Rate of Return** (**RoR**): $\frac{\text{payout}-\text{bet}}{\text{bet} \times 100}$
- **Weighted Probability**: The implied probabilities of winning are 64% for the White Queen and 36% for the Red Queen

In conclusion, the basics of pari-mutuel betting are:

- The expected return (weighted by the probabilities) is 0%, this is called a *fair gamble* which equates to neither winning nor losing on average
- In practice, there is usually a tax on pari-mutuel betting, and so the expected return is negative
- A punter who believes he can make money from gambling believes that the true probabilities are different from the probabilities implied by the bets of all other punters

#### Bookmaking
The key points of bookmaking are the following:

- A bookmaker is someone who takes bets from punters for profit
- Bookmakers offer odds to punters that imply a rate of return on bets
- A bookmaker can adjust the odds offered so that the expected payout is the same regardless of the actual outcome (a *balanced book*). A balanced book will have odds whose implied probabilities are the same as in the case of the pari-mutuel example
- A bookmaker profits by offering odds which imply the outcome is more likely than it really is, so that the implied total probability is >100%. This is called the **overround** or **vig**
- A bookmaker that operates a balanced book is therefore guaranteed a profit equal to the vig
- In practice, many bookmakers take a *position*; meaning they may win or lose money based on the outcome
- To beat the bookmaker and make a profit, the punter not only needs to believe that the gap between the true probability and the bookmaker odds is larger than the vig, but also greater than the tax on betting

#### Betting Exchanges
The key points of betting exchanges are the following:

- In the internet era, betting exchanges have become a popular alternative to bookmakers
- A betting exchange matches punters with opposing opinions on outcomes based on the odds. Thus one punter may offer a bet at given odds, and another punter can bet against them by accepting the match.
- Betting exchanges take a commission on matching bets
- Exchanges offer more flexibility in terms of the bets that can be made; however, the market is also somewhat more complex and so the beginner is generally better off starting with a bookmaker

#### Conclusions
- Gambling is a type of market where punters compete by staking money on different outcomes
- In these markets the odds on each possible outcome represent probabilities
- The pari-mutuel betting example shows how these probabilities can be inferred by the weight of money placed on that outcome
- While bookmaking and betting exchanges work differently, the same concept applies; *the weight of money implies probability*

### Betting Odds and Types of Bets
Betting odds are defined by how much money you will receive if you win your bet. Odds can be expressed in different ways and the 3 most common expressions are traditional, decimal and moneyline.  The following table is taken from a betting exchange to show an example of how each is represented.

| Contest | Odds Method | Team 1 Odds | Team 2 Odds |
| :-- | :-: | :-: | :-: |
| Miami Heat - Philadelphia 76ers | Traditional | 39/100 | 53/25 |
| Miami Heat - Philadelphia 76ers | Decimal | 1.39 | 3.12 |
| Miami Heat - Philadelphia 76ers | Moneyline | -256 | +212 |

1. Traditional/British Odds <br>
    - Expressed as a ratio of what you stake to what you return
    - 39/100 means that for every \\$100 that you stake, you return \\$39 in addition to your stake (i.e. \\$139)
    - This implies that the bookmaker's probability that Miami wins is $Pr(\text{Miami})=\frac{100}{100+39}=0.719$
2. Decimal/European Odds <br>
    - Express the payout of a bet as a ratio of the stake, where the stake is included in the payout
    - A bet on Miami returns 1.39x the original bet
    - Converting to probability is simply $Pr(\text{Miami})=\frac{1}{1.39}=0.719$
3. Moneyline/American Odds <br>
    - Expressed as a positive or negative integer
        - If positive, they state the amount of money returned for a stake of \\$100
        - If negative, they state the amount of money to be staked to win \\$100
    - A bet on Miami requires a \\$256 stake to win \\$100 (returns \\$356)
    - The calculation of implied probability depends on whether the value is positive or negative
        - If positive, $Pr(\text{Phila})= \frac{100}{212+100} = 0.321$
        - If negative, $Pr(\text{Miami})= \frac{-(-256)}{100-(-256)} = 0.719$

### Betting Odds and Win Probabilities

### Evaluating Betting Odds Using Brier Scores

### Market Efficiency and Beating the Bookmaker
If the possibility of *beating the bookmaker* exists, it contradicts the **Efficient Market Hypothesis** (**EMH**).  This hypothesis was developed with the stock market in mind and states that:

*Stocks always trade at their fair value on exchanges, making it impossible for investors to purchase undervalued stocks or sell stocks for inflated prices. Therefore, it should be impossible to outperform the overall market through expert stock selection or market timing, and the only way an investor can obtain higher returns is by purchasing riskier investments.*

Many believe that this same hypothesis applies to sports betting as well.  Despite the belief that *it is not possible to defeat the bookmaker*, a few of the following strategies have proven successfull:

- Generate a strategy based on a model which has been calibrated using historical data and then "tested" against a subset of data not used to create the strategy
- Such models are usually based on statistical methods such as the logit regression model, but also require "expert judgment" to account for non-quantifiable factors
- Strategize to lay a bet when the difference between the bookmaker odds and the model probabilities is large enough
- The higher the threshold, the fewer profitable bets that exist, so the strategy balances profitability with frequency to generate the max profit over some period
- All strategies ***must*** have a stopping point. No model is going to be profitable forever!!
