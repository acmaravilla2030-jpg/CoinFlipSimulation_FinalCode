# CoinFlipSimulation_FinalCode


## Coin Flip Simulator (v1.1.0)
A Python-based utility designed to model stochastic processes through simple Bernoulli trials. This project supports standard simulations, weighted probability experiments for statistical testing, and a "Double or Nothing" betting game.


## Features
• Standard Simulation: 
  -Quick 50/50 coin toss modeling.
• Weighted Probability Engine: 
  -Simulate biased coins (e.g., 70% heads) to see how probability shifts over large datasets.
• Data Export (CSV): 
  -Automatically logs individual flip results to coin_results.csv for analysis in Excel or Google Sheets.
• Double or Nothing Mini-Game: 
  -A CLI-based betting game with a persistent balance tracker.
• Performance Optimized: 
  -Includes a PRINT_LIMIT to prevent console lag during massive simulations (e.g., 1,000,000+ flips).

## Code:
https://onlinegdb.com/P4_Ri2-2I

## How to Run on OnlineGDB
1.	Ensure the language is set to Python 3.
2.	Click the Run button (or press F9).
3.	Follow the on-screen menu prompts to choose your mode.
4.	To access exported data: After running a simulation with export enabled, check the "Files" tab in the side panel to download coin_results.csv.

## Step-by-step walkthrough of the terminal interaction

## 1. The Main Menu
This is the "home base" that appears when you start the script.

====== Coin Flip Simulator ======
1. Standard Simulation
2. Weighted Coin Experiment
3. Double or Nothing Game
4. Exit
Choose an option: 

## 2. Standard Simulation (Option 1)
If you choose 10 flips and say "y" to export, the output looks like this:

How many flips? 10
Export results to CSV? (y/n): y

Running simulation...

Flip 1: Heads
Flip 2: Tails
Flip 3: Heads
... (etc) ...
Flip 10: Tails

--- Simulation Summary ---
Total flips: 10
Heads: 6 (60.00%)
Tails: 4 (40.00%)
Results exported to: coin_results.csv

(Note: If you entered 100 flips, it would skip the "Flip X: Result" lines to keep your screen clean because of the PRINT_LIMIT.)


## 3. Weighted Experiment (Option 2)
This is where you rig the coin. If you set the probability to 0.8 (80% Heads):

How many flips? 100
Probability of Heads (0-1): 0.8
Export results to CSV? (y/n): n

Running simulation...

--- Simulation Summary ---
Total flips: 100
Heads: 82 (82.00%)
Tails: 18 (18.00%)


## 4. Double or Nothing Game (Option 3)
This is interactive. The program waits for your input after every flip.

--- Double or Nothing Game ---
Starting balance: 100
Enter bet amount (0 to exit, Max 100): 50
Coin result: Heads
You won!
Current balance: 150

Enter bet amount (0 to exit, Max 150): 150
Coin result: Tails
You lost!
Current balance: 0

Bust! You're out of money.
Game over. Final balance: 0


## Summary of User Input Types
• Menu: String/Text (1, 2, 3, or 4)
• Counts: Integers (10, 500)
• Probability: Floats (0.5, 0.75)
• Decisions: Characters (y or n)



