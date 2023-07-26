# Hospital Bed Management with Reinforcement Learning

Hospital Bed Management with Reinforcement Learning is a Python implementation of a bed management system for hospitals using reinforcement learning techniques. The system aims to optimize the allocation of available beds for normal and COVID-19 patients, taking into account the number of incoming requests and returns over a given period.

## Key Components

1. `Hospital`: Represents the hospital with the number of available beds for normal and COVID-19 patients, initial bed counts, and other parameters like the maximum capacity and discount rate.
2. `poisson_`: Implements a custom class to handle Poisson distributions and their probabilities for optimization purposes.
3. `Beds`: Represents the available and returning beds based on the number of requests and returns, using Poisson distributions.
4. `Agent`: Defines the agent responsible for policy improvement and calculating the expected rewards for different actions.
5. `policy_improvement`: The method for policy iteration, aiming to stabilize the optimal bed allocation policy.

## Usage

1. Create a `Hospital` object by providing the initial number of available beds, the maximum hospital capacity, and the discount rate.
2. Create an `Agent` object with the hospital information, an empty value matrix, an empty policy matrix, and a constant for the expected value.
3. Run the policy improvement loop to optimize the bed management policy.

## Dependencies

- numpy
- scipy
