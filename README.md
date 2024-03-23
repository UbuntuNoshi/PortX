# PortX

## Effective deFi portfolio management.

This is a pure quant aproach. Yes there are qualitative approaches.
But the scope of this project is pure portfolio quants and incorporating AI.


...to effectively allocate to the best assets at the best quantities, needs
large compute. And why not be able to go directly to the market without a
middleman charging you an annual fee? LFG DeFi.


Yes, we are going to disrupt the investment management industry.
The aim is to get the most return for the least risk and outperform some benchmark.
And middlemen are too expensive.

The goal:
Max(active risk adjusted return) after fees.

---

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

Return | Relativity = Active Return

This dimension is commonly called alpha*. It is the outperformance of one asset
over another, or a group of assets over another group of assets ussually called
an index or benchmark. 

*Active risk-adjusted retun is a superior measure but we are systematically getting there.

Risk | Exposure = Contribution to risk

Squareroot of the assets weight squared times its standard deviation squared
plus the interaction part of the formula which is the 
squareroot(2*wi*wj*stdevi*stdevj*correlij) between each asset.

Risk | Relativity = Active risk

Much like active active return but it gauges the 
excess risk one or a group of assets have to another asset or group. Beta is the normal 
measure but the difference in risk can also be used.

Exposure | Relativity = Relative bets

Example is easier.
Suppose you have A, set of assets, and B another set of assets.
Weight of asset in A minus weight of asset in B.
Where a not element of B, relative bet > 0
Where b not element of A, relative bet < 0
where A is the asset/group of assets measured against asset or group 
of assets B, ussualy an benchmark or index.

### On the introduction of the third generation dimensions (TGD):

Contribution to return | Contribution to risk | Risk adjusted return = Contribution to risk adjusted return

This is a dimension to see which assets contributed how much to the sharpe ration. It is a stronger insight
as risky assets might not yield the performance to justify risking that much capital of the portfolio.

Contribution to return | Relative bets | Active return = Contribution to active return

*

Contribution to risk | Relative bets | Active risk = Contribution to active risk

*

Active return | Active risk | Risk adjusted return = Active risk adjusted return

*


























