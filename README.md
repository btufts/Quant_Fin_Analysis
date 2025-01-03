# Quant_Fin_Analysis

Quantitative financial analysis code. Analysis of 4 strategies optimized for 10 currency pairs and robustness tested using 3 different methods. Many of the docstrings were assisted by Codeium.

## Repo Map

### Reproductions

This folder includes a list of jupyter notebooks. Each notebook includes a link to the source of the strategy and the original backtesting results from that source. It is followed by my recreation of that strategy and 3 of my backtests on that strategy. The first backtest has no Cheat On Open or Cheat On Close. This is the most realistic backtest. The second includes Cheat On Open. This is slightly less realistic as it gaurantees you get to buy on the next open price which is unlikely. The last includes Cheat On Close. This is the most unrealistic backtest because you can't possibly buy on a days close price. However, in some cases that is the backtest that lines up the most with the original source backtest so I include it.

**Disclaimer: I did not pay for anything on the source strategy websites. As a result not all of the details about the strategies are divulged, which results in some discrepancies between my backtest and the sources.**

### Data

Folder containing all of the yahoo finance data necessary to reproduce the results. New data files do not have to be stored in this folder so long has the correct path is specified when running main files.

### Reports

Final_Backtesting_Report and Final_Robustness_Report are two reports written using these files and data. The provide enough detail to recreate all of the results shown in the reports.

### Tests

Test files for various functions. Many functions rely heavily on backtrader and are therefore not tested by me because I couldn't possibly build test cases without using backtrader which would... well defeat the purpose of the test.

Most of the tests were assisted by GPT-4o.

### Main Files

The two main files to run are  robustness_report.y and strategy_report.py. The bash files starting with run provide examples of how to use these scripts. Strategy report does backtesting and optimizing. Robustness reports evaluates the robustness of the strategy.

Graphs.ipynb show visuals of the optimization universes created by strategy_report.py.