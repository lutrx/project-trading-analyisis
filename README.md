# Trading strategy analysis | Mid-bootcamp project

**Lisa-Maria Bieker**
**Ironhack Data Analysis**

## Topic

The aim of this project was to disprove the Random-Walk-Theory. Therefore, three trading strategies were checked with different forex trading pairs (daily and minute data). 

The following strategies were tested:
1) Red green candle
2) Reversed candle
3) Moving average crossover

Trading pairs: USDJPY, EURUSD, GBPUSD, USDCAD

Presentation of the project was done with Google slides: [link](https://docs.google.com/presentation/d/1PZe9e99hSPyGy4r6Np3WpFqlSk9mLt3SleRImtloFlo/edit?usp=sharing)

## The following tools/skills were used:

  * Jupyter Notebook
  * Python: Pandas, Numpy, Seaborn, Matplotlib
  * MySQL
  * Tableau
  * Statistical analysis

## Dataset

Data was used from these sources:

  * [Daily data](https://stooq.com/db/h/)
  * [Daily and minute data](https://www.interactivebrokers.com/en/home.php)

All datasets contained the following columns:

  * Date/time
  * Open
  * High
  * Low
  * Close
  * Volume

## Preparation of data and testing of strategies

  * dropping of not required columns (volume etc.)
  * conversion of data in ticks
  * calculation of difference open - close prices per row
  * calculation of classification and order type columns (long, short, none) depending on strategy per row
  * calculation of profit per row
  * preparation for figures: calculation of cumulative profit per row
 
 ## Analysis and visualization
 
  * calculation of how many standard deviations result of strategy is away from expected profit value of 0 --> significance level for accepting strategy 
    as valid is 3.9 standard deviations
  * analysis of number of trades vs cumulative profit: Tableau and Matplotlib

## Conclusion

Adapted red green strategy in combination with USDJPY minute data resulted in a profitable strategy with a standard deviation of 5.22. Under the given significance level and by usage of this strategy and dataset the Random-Walk-Theory could be disproved.

