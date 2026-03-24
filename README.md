# CoinFlipSimulation_FinalCode


## Coin Flip Simulator (v1.1.0)
A Python-based utility designed to model stochastic processes through simple Bernoulli trials. This project supports standard simulations, weighted probability experiments for statistical testing, and a "Double or Nothing" betting game.


## Features
• Standard Simulation: Quick 50/50 coin toss modeling.
• Weighted Probability Engine: Simulate biased coins (e.g., 70% heads) to see how probability shifts over large datasets.
• Data Export (CSV): Automatically logs individual flip results to coin_results.csv for analysis in Excel or Google Sheets.
• Double or Nothing Mini-Game: A CLI-based betting game with a persistent balance tracker.
• Performance Optimized: Includes a PRINT_LIMIT to prevent console lag during massive simulations (e.g., 1,000,000+ flips).


## How to Run on OnlineGDB
1.	Ensure the language is set to Python 3.
2.	Click the Run button (or press F9).
3.	Follow the on-screen menu prompts to choose your mode.
4.	To access exported data: After running a simulation with export enabled, check the "Files" tab in the side panel to download coin_results.csv.
