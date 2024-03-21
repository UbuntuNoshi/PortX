# PortX

## Effective deFi portfolio management.

Why deFi? To effectively allocate to the best assets at the best quantities, needs
large compute. And why not be able to go directly to the market? 
Yes, we are going to disrupt the investment management industry.
The aim is to get the most return for the least risk and outperform some benchmark.
Max(active risk adjusted return)

## The theory:

### On the introduction of the base dimensions (BD):

Risk and return are the first two base dimensions, 
where the latter gets more attention.
Risk, in recent years have gathered more attention.
Each asset has a return and risk profile. Return is calculated by the percentage
change in price from time 0 to time 1. Risk is the standard deviation of a set of these
returns.

When one has a portfolio of these risk and return profiles,
one has to assign weights to each asset. This brings us to
the third base dimension, namely exposure. Exposure always sums up to one
for the portfolio, where shorts are < 0 and longs > 0.

The last base dimension is something I are calling relativity. 
This is how one asset compares to another or a portfolio to a benchmark.
Intra portfolio it is done by the co-variance between assets. Inter portfolios
we focus on differences between risk, return and exposures.

### On the introduction of the second generation dimensions (SGD):

I arrive at the SGDs by taking a permutation of the BD in sets of two.

Return | Risk = Risk adjusted performance
The idea here is to compare apples with apples. An asset with large volatility (downside)
and large return is comparable with a  low return asset with low volatility (downside).
This is the Sharpe ratio.

Return | Exposure = Contribution to performance
Return of the portfolio is the sum of all the weights times each assets's performance.
This weighted return gives insight into the drivers of the portfolio's performance.

Risk | Exposure = Contribution to risk
Squareroot of the assets weight squared times its standard deviation squared
plus the interaction part of the formula which is the 
squareroot(2*wi*wj*stdevi*stdevj*correlij) between each asset.




