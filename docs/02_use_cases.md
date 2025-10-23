### Use Case ID: UC-01
**Use Case Name:** Run Monte Carlo Simulation

**Primary Actor:** Users
**Goal:** Generate a probabilistic forecast of portfolio value over time under user-defined and stochastic conditions

**Preconditions:**
- User has launched the Monte Carlo Simulation.
- Historical and Synthetic Data is accessible. 

**Main Flow:**
1. User enters portfolio details.
    - Total Amount Invested 
    - Asset's Ticker
    - Asset Percentage in Portfolio
    - Repeat until portfolio is complete 
2. User selects Monte Carlo simulation settings.
    - Number of Simulations
    - Duration of Simulations (Months or Years)
3. User checks whether to enter include **Black Swan scenarios.**
    - If yes, user is prompted to enter potential **Black Swan Scenario**
4. Simulation validates user inputs.
5. Simulaions runs Monte Carlo iterations based on settings.
6. Simulation Returns 5 benchmark scenarios and summary statistics.
    - Best Case Scenario
    - Above Aversge Scrnario
    - Average Scenario
    - Below Average Scenario
    - Worst Case Scenario
    - Distribution of Outcomes
7. User may save, compare or export the results.

**Post-Conditions:**
- Simulations are stored locally or in the user's profile.
- Ouput visualizations and summary metrics are accessible.

**Alternative Flows:**
- (A1) Invalid input -> System displays appropriate error message.
- (A2) Missing Data -> System prompts them to enter needed data.