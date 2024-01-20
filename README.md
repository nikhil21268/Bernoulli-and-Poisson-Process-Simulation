# Bernoulli and Poisson Process Simulation
## Stochastic Processes and Applications Assignment 
Wrote Python Code to simulate Bernoulli and Poisson Processes.

# Problem Statement

## Introduction

This problem involves simulating and analyzing random processes modeled as Bernoulli and Poisson processes using basic functions in R or Python. The tasks include simulating coin tosses and hospital emergency room arrivals, visualizing the results through histograms and graphs, and comparing outcomes under different parameter values.

## Problem Details

### Task 1: Bernoulli Process Simulation (10 points)

Suppose a coin is tossed 20 times, and the process is modeled as a Bernoulli process with a success probability (p) of 0.8.

#### Subtask (a)

- **Objective:** Simulate the process 1000 times and visualize the results using a histogram.
- **Expected Output:** A histogram depicting the distribution of successes in the simulated process.

#### Subtask (b)

- **Objective:** Repeat the simulation for p = 0.5 and compare the results with Subtask (a).
- **Expected Output:** A histogram comparing the distributions for p = 0.8 and p = 0.5.

### Task 2: Poisson Process Simulation (15 points)

Assume patients arrive at a hospital's emergency room at a rate of 5 patients per hour, modeling it as a Poisson process.

#### Subtask (a)

- **Objective:** Simulate the density of the number of arrivals until time t and verify the mean value.
- **Expected Output:** Graph(s) illustrating the density of arrivals and a verification of the mean value.

#### Subtask (b)

- **Objective:** Repeat the simulation for λ = 15 and compare the results with Subtask (a).
- **Expected Output:** Graph(s) comparing the densities for λ = 5 and λ = 15.

#### Subtask (c)

- **Objective:** Simulate the first inter-arrival time of the process and provide related graph(s).
- **Expected Output:** Graph(s) illustrating the distribution of the first inter-arrival time.



# Coin Toss Bernoulli Process

## (a) Probability of Success (p = 0.8)

In this simulation, we model the coin toss process as a Bernoulli process with a probability of success (p) set to 0.8. This means that each coin toss has a higher chance of resulting in a "heads." The simulation involves tossing the coin 20 times in each of the 1000 experiments.

### Inference from the Plots

The average number of heads can be approximated as \(n \times p\), where:
- \(n\) is the number of coin tosses (20 in this case).
- \(p\) is the probability of success (0.8 for part (a)).

Theoretical Reasoning:

Recall that the Moment Generating Function (MGF) of a Bernoulli random variable is \(M_{X_i}(t) = pe^t + (1-p)\). The MGF of the sum of \(n\) independent Bernoulli random variables is the MGF of a Binomial random variable with parameters \(n\) and \(p\).

### Observations

For part (a), where \(p = 0.8\), the average number of heads is approximately 16 based on the simulation.

## (b) Probability of Success (p = 0.5)

In this case, we set the probability of success (p) to 0.5, making the coin toss a fair one. The simulation involves tossing the coin 20 times in each of the 1000 experiments.

### Inference from the Plots

The average number of heads can be approximated as \(n \times p\), where:
- \(n\) is the number of coin tosses (20 in this case).
- \(p\) is the probability of success (0.5 for part (b)).

### Observations

For part (b), where \(p = 0.5\), the average number of heads is approximately 10 based on the simulation.

## Summary

In summary, the plots and theoretical reasoning confirm that a higher value of \(p\) results in a higher probability of success in each trial, leading to a greater average number of successes in the coin toss simulations.

# Hospital Emergency Room Poisson Process

## (a) Rate Parameter (λ = 5)

For a Poisson process with a rate parameter of 5 patients per hour, we simulate the number of arrivals in a specific time interval (0, t]. The expected average number of arrivals in one hour is 5, and we verify this through simulation.

### Observations

In this simulation, with a time interval of 10 hours, the mean number of arrivals is approximately 50.

## (b) Rate Parameter (λ = 15)

Increasing the rate parameter to 15 implies an expected average of 15 patients per hour. We compare the results with the previous simulation where \(λ = 5\) for the same time interval.

### Observations

For the simulation with \(λ = 15\) and a time interval of 10 hours, the mean number of arrivals is approximately 150.

## (c) First Inter-Arrival Time

The first inter-arrival time in a Poisson process, modeled by an exponential distribution, represents the time until the first patient arrives at the emergency room. Simulations are conducted for different rate parameters.

### Observations

The plots illustrate the distribution of the first inter-arrival time, confirming the typical exponential decay pattern.

## Theoretical Reasoning

To support the observations, theoretical reasoning includes derivations of the mean value of the number of arrivals in a Poisson process and the proof that the inter-arrival times follow an exponential distribution.

Note: All graphs and additional details can be found in the accompanying `.ipynb` file uploaded with the assignment.
