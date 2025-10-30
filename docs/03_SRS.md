# Software Requirements Specification (SRS)
## Monte Carlo Portfolio Simulator

### 1. Introduction

#### 1.1 Purpose
This document specifies functional and non-Functional requirements for the Monte Carlo portfolio simulator - a Python-based application that models potential portfolio outcomes using stocahsfic models.  

#### 1.2 Scope
The simulator enables users to:
- Configure portfolio with custom assets and their portfolio weight
- Run monte carlo simulations using historic or generated data
- Visualize probablististic outcomes for portfolio based on configurations and export results 

1.3 Definitions, Acroynms, and Abbrevations
- **Monte Carlo Simulation** - Statisticsl modeling technique using random sampling
- **Black Swan** - Rare, extreme market event causing significant deviation
- **Portfolio** - A collection of assets with user-defined weights

1.4 References
- [Problem Statement](./01_problem_statement.md)
- [Use Cases](./02_use_cases.md)
- Python Libraries: NumPy, Pandas, Matplotlib 

### 2. Overall Description

#### 2.1 Product Perspective
This is a standalone simulation tool designed for learning and research use 

#### 2.2 Product Functions
- Input portfolio details
- Add potential black swan event
- Run thousands of future outcomes 
- Display result's visualization and summary
- Allow user to save and export results

2.3 Constraints
- Dependent on open-source python library 
- Python 3.12+

### 3. Specific Requirements

#### 3.1 Functional Requirements
- FR-1 | Allows user to input portfolio details | High
- FR-2 | Allows user to include potential black swan events | Medium
- FR-3 | Run Monte Carlo Simulations | High
- FR-4 | Display percentile distrubtion and charts | High
- FR-5 | Save/Export Results | Medium

#### 3.2 Non-Functional Requirements
- NFR-1 | Performance | 10,000 simulations must be completed in <= 5seconds | High
- NFR-2 | Usability | User can run simulation in <= 3steps
- NFR-3 | Reliabiliy | Consistent results for fixed random seed
- NFR-4 | Portability | Works in Windows, MacOS, and Linux