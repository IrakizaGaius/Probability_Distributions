# Assignment on Probability Distributions, Bayesian Probability, and Gradient Descent Implementation

This repository showcases an assignment on the following topics:

- **Probability Distributions**
- **Bayesian Probability**
- **Gradient Descent Implementation**

## Overview

This repository focuses on various concepts related to probability distributions, with a specific implementation of **Exponential Probability Distribution**. The key goal of this assignment is to demonstrate and simulate real-world scenarios using probability distributions, and apply methods like Bayesian Probability and Gradient Descent for analysis.

### File Breakdown

#### `exponential.py`

This file showcases the implementation of a **real-world example** using the **Exponential Distribution**.

#### Scenario

A large cloud computing company manages a data center where servers receive incoming network packets. The arrival of these packets follows an Exponential distribution due to the following reasons:

- Packets arrive **randomly and independently**.
- The **rate of incoming packets** remains constant over time.

#### Problem Statement

- The average packet arrival rate is **500 packets per second**.
- The task is to simulate and visualize the distribution of **inter-arrival times** (time between consecutive packets).
- We aim to check if the **empirical data** (simulated values) matches the **theoretical Exponential distribution**.

#### Goals

- Simulate the random arrival of network packets.
- Compare the simulated data with the theoretical Exponential distribution to see how well they align.
  
## Requirements

- Python 3.x
- Libraries:
  - `numpy`
  - `matplotlib`
  - `scipy`

## Running the Code

1. Clone the repository to your local machine:

   ```bash
   git clone <repository-url>
   pip install -r requirements.txt
   python exponential.py

### Report Insights for our Real worlsd example(exponential.py)

**How does the distribution you were allocated vary from the other three you were not allocated?**

-**The Exponential distribution** models the time between consecutive events in a Poisson process, such as the time between packet arrivals in a data center. This contrasts with the other distributions:

- **Normal Distribution** is symmetric and models data around a mean, which doesn’t fit the nature of inter-arrival times that are skewed (with shorter times more frequent and longer times less so).

- **Poisson Distribution** models the number of events in a fixed interval of time, but in this case, the focus is on the time between events, making Exponential a better fit.

- **Binomial Distribution** models the number of successes in a fixed number of trials, which is not applicable for modeling continuous random events like packet arrivals.

**Would the question you chose be used in the context of a different distribution?**

No, the scenario of packet arrivals is best suited to the Exponential distribution, as it captures the random and independent arrival times at a constant rate. The Normal, Poisson, and Binomial distributions do not fit well because they either model counts of events or symmetrical distributions, which don’t align with the time-based nature of this problem.
