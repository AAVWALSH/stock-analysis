# Refactoring Code to Better Analyse Stocks in VBA
## Module 2 VBA stock analysis


### Overview of Project
The goal of this project was to analyse the performance of a set of 12 stocks over two years. We developed a table to quickly show the user that each individual stock's Total Daily Volume was and then the percentage return on investment. With the press of a button the user can receive a visualization of the returns.

While an initial functioning code was build it was then refactored to perform more efficiently.

### Results
#### The Stocks
The 2017 stock results show significant positive returns on investments. The following year 2018 proves the old investment addage that 'past performance does not predict future results' as most stocks performed negatively. 
Here are the two years:
![2017 stocks](/../main/stock-analysis/Resources/2017_stocks.png)

(https://github.com/AAVWALSH/stock-analysis/blob/a439cc4d35bf48849510341111a928ca24c04e21/Resources/2017%20stocks.png)
![2018 Stocks](https://github.com/AAVWALSH/stock-analysis/blob/a439cc4d35bf48849510341111a928ca24c04e21/Resources/2018%20stocks.png)

#### The Code
The refactored code performed significantly faster than the originally written macros.The refactored macro took all the subroutines created separately and combined it into one complete block in a new module so that each line as looped through once.

As a result of refactoring the runtime was cut significantly. In the original the 2017 stocks took 1.75 seconds and 2018 took 1.89 seconds. While that does not generally seem like a long time the larger the dataset the more time it would take. After refactoring 2017 ran in .23 seconds and 2018 ran in .26 seconds.

![Runtime after refactoring 2017](https://github.com/AAVWALSH/stock-analysis/blob/a439cc4d35bf48849510341111a928ca24c04e21/Resources/VBA_Challenge_2017.png)

![Runtime after refactoring 2018](https://github.com/AAVWALSH/stock-analysis/blob/a439cc4d35bf48849510341111a928ca24c04e21/Resources/VBA_Challenge_2018.png)

### Summary
The obvious advantage of refactoring code is the more efficient runtime. This only gains in importance as the datasets grow in size and complexity. One negative is the time it can take to create the more efficient code. There may be a feeling of "if it's not broken why fix it?". The more complex of a file you're working with the easier it would be to make an error that would effect the functioning of the program. The analyst must determine whether the time spent refactoring is worth the overall time and effort. If the dataset is small or will only be used sparingly then a clunkier but working code may suffice. If, however, the project needs to be scaled up in size, collaborated on with others, shared with others, or used frequently then every care should taken to create precise, well commented, and slim-lined code. 
