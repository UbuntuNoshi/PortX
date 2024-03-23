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

## On the introduction of the base dimensions (BD):

Risk (R) and performance (P) are the first two base dimensions, 
where the latter gets more attention.
Risk, in recent years have gathered more attention.
Each asset has a return and risk profile. Return is calculated by the percentage
change in price from time 0 to time 1. Risk is the standard deviation of a set of these
returns.

When one has a portfolio of these risk and return profiles,
one has to assign weights to each asset. This brings us to
the third base dimension, namely exposure (E). Exposure always sums up to one
for the portfolio, where shorts are < 0 and longs > 0.

The last base dimension is something I are calling relativity (Re). 
This is how one asset compares to another or a portfolio to a benchmark.
Intra portfolio it is done by the co-variance between assets. Inter portfolios
we focus on differences between risk, return and exposures.

## On the introduction of the second generation dimensions (SGD):

I arrive at the SGDs by taking a permutation of the BD in sets of two.

P | R = Risk adjusted performance

The idea here is to compare apples with apples. An asset with large volatility (downside)
and large return is comparable with a  low return asset with low volatility (downside).
This is the Sharpe ratio.

P | E = Contribution to performance

Return of the portfolio is the sum of all the weights times each assets's performance.
This weighted return gives insight into the drivers of the portfolio's performance.

P | Re = Active Return

This dimension is commonly called alpha*. It is the outperformance of one asset
over another, or a group of assets over another group of assets ussually called
an index or benchmark. 

*Active risk-adjusted retun is a superior measure but we are systematically getting there.

R | E = Contribution to risk

Squareroot of the assets weight squared times its standard deviation squared
plus the interaction part of the formula which is the 
squareroot(2*wi*wj*stdevi*stdevj*correlij) between each asset.

R | Re = Active risk

Much like active active return but it gauges the 
excess risk one or a group of assets have to another asset or group. Beta is the normal 
measure but the difference in risk can also be used.

E | Re = Relative bets

Example is easier.
Suppose you have A, set of assets, and B another set of assets.
Weight of asset in A minus weight of asset in B.
Where a not element of B, relative bet > 0
Where b not element of A, relative bet < 0
where A is the asset/group of assets measured against asset or group 
of assets B, ussualy an benchmark or index.

### On the introduction of the third generation dimensions (TGD):

P | R | E = Contribution to return | Contribution to risk | Risk adjusted return = Contribution to risk adjusted return (CRAR)

This is a dimension to see which assets contributed how much to the sharpe ration. It is a stronger insight
as risky assets might not yield the performance to justify risking that much capital of the portfolio.

P | Re | E = Contribution to return | Relative bets | Active return = Contribution to active return (CAR)

This dimensions measures the build up of difference in performance between two or group of assets.

R | Re | E = Contribution to risk | Relative bets | Active risk = Contribution to active risk (CARk)

This dimensions measures the build up of difference in risk or beta between two or group of assets.

P | R | Re = Active return | Active risk | Risk adjusted return = Active risk adjusted return (ARAR)

This is the group of assets' goal; maximise the the relative performance while minimising the relative
risk between two or two groups of assets. At this stage we are not looking at the breakdown per asset.
That's the next and final generation of dimensions.

### On the introduction of the fourth generation dimensions (FGD):

P | R | Re | E = CRAR | CAR | CARk | ARAR = Contribution to active risk adjusted return

Finally when can see where the quantitative risk and performances comes from which assets 
versus a asset or group of assets.


---

p.s. there are one more base dimension, namely time, but for simplicity
sake I have left this out for now. It simply means one of two things, 

at each point in time the above dimensions would have a set of values, except at time zero.
and the time horison or interval of the measurements of performance and risk.






















