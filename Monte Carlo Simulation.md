Monte carlo simulation used to model the probability of different outcomes using random variable, it is commonly used to understand the impact of risk and uncertainty.

Use random sampling to obtain numerical result for mathematical problem that may be deterministic in principle but are difficult to solve analytically.

Basically start with random sampling and repeated for a bunch of times, the result then aggregated to produce a probability distribution of the outcome.

## Application
Used in many fields including investing, business, physics, and engineering. Monte Carlo simulation often referred as multiple probability simulation
 
In finance, it usually used for risk assessment, option pricing, and portfolio management. It also can be used for modelling the uncertainty of market price, interest rate, and other financial variables.

## Notes
- Monte carlo simulations assume perfectly efficient markets. (efficient market is when asset price reflect all information both public and insider, thus insider information cannot give investor an advantage in predicting price movement)

## 4 Steps of Monte Carlo Simulation
Two components of an asset's price movement:
1. Drift, constant directional movement.
2. Random input, which is the market volatility.

By analyzing historical data you can determine the drift, std, and variance, and the average price movement of a security. These are the building block of Monte Carlo simulation.

STEP 1
To predict possible price trajectory, using the historical price data of an asset to generate a series of periodic daily return using natural logarithm.

$Periodic Daily Return$=$ln$ $($$Day's Price \over Previous Day's Price$$)$

STEP 2
Use AVERAGE, STDEV.P, and VAR.P on the entire resulting series to obtain the average daily return, standard deviation, and variance input.

$Drift$=$Average Daily Return$-$Variance \over 2$

Average Daily Return = From excel
AVERAGE function from periodic daily return series
Variance produce from excel
VAR.P function from periodic daily return series

STEP 3
Obtaining a random input

$Random Value$=$σ \times NORMSINV(RAND())$

Next is the equation fore the following day's price:

$Next Day's Price$=$Today's Price \times e^{(Drift+Random Value)}$

STEP 4
To take e to a given power, use EXP function

## Monte Carlo Simulation Result
The frequencies of different outcomes generated will form a normal distribution. The most likely outcome is in the middle of the curve, meaning there is an equal chance that the actual return will be higher or lower.

For within one standard deviation is the probability is 68%, 95% within two standard deviation, and 99.7% within three standard deviation.

Monte carlo Simulation ignore everything not built into the price movement, such as macro trends, company leadership, market hype, and cyclical factors, in other words assuming efficient market.

## Advantage and Disadvantage of Monte Carlo Simulation
- Help investor estimate likelihood of gain or loss of certain investment.
- Monte Carlo test a number of random variables then average(aggregate) rather than starting out with the average

