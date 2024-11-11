# Reinforcement-Learning

This repository contains a collection of classic Reinforcement Learning (RL) algorithms, implemented using Python and the [Gym library](https://www.gymlibrary.dev/). These algorithms demonstrate fundamental approaches to decision-making and learning in environments with uncertain outcomes and are applied to various benchmark environments. 

The [Gym library](https://www.gymlibrary.dev/) is a toolkit for developing and comparing RL algorithms. It provides a diverse collection of environments, including classic control problems and grid-based challenges, which makes it an excellent framework for experimenting with RL algorithms.

---

## Contents

### Algorithms and Implementations

1. [**Policy Iteration (Frozen Lake Environment)**](Policy_Iteration_Frozen_Lake.ipynb)  
   Policy iteration iteratively evaluates and improves a policy until it converges to the optimal policy. This method is applied to `FrozenLake`, where the agent learns a policy that maximizes expected rewards in a slippery, frozen environment.

2. [**Value Iteration (Frozen Lake Environment)**](Value_Iteration_Frozen_Lake.ipynb)  
   Value iteration is a dynamic programming method that computes the optimal value function iteratively until convergence. Applied in `FrozenLake`, it enables the agent to find the optimal policy by directly optimizing state values.
   
3. [**Q-Learning (Frozen Lake Environment)**](Q_Learning_Frozen_Lake.ipynb)  
   Q-learning is a model-free RL algorithm that updates Q-values based on the highest estimated future reward. Applied to `FrozenLake`, this implementation teaches the agent to navigate and reach the goal despite environmental challenges.

4. [**Q-Learning (Cliff Walking Environment)**](Q_Learning_cliff_walking.ipynb)  
   This Q-learning implementation tackles the `CliffWalking` environment, where the agent learns to navigate between a start and goal while avoiding falling off the cliff. The algorithm prioritizes exploration and learns from past actions to maximize cumulative reward.

5. [**Double Q-Learning (Frozen Lake Environment)**](Double_Q_Learning_Frozen_Lake.ipynb)  
   This algorithm uses Double Q-learning to improve stability in learning by maintaining two separate Q-value tables, minimizing the overestimation bias found in standard Q-learning. Applied to the `FrozenLake` environment.   

6. [**SARSA (Cliff Walking Environment)**](Sarsa_cliff_walking.ipynb)  
   SARSA (State-Action-Reward-State-Action) is an on-policy method, which means the updates follow the policy being used by the agent. Applied in `CliffWalking`, this approach emphasizes a safe path over high-reward but risky actions, learning from current policy actions rather than the greedy choices.

7. [**Dyna-Q (Custom Maze)**](Dyna_Q.ipynb)  
   Dyna-Q is a hybrid approach that combines Q-learning with model-based planning, where the agent builds a model of the environment and uses simulated experiences. Here, Dyna-Q is implemented in a self-made maze environment with custom rules, demonstrating its adaptability in both known and unknown settings.
