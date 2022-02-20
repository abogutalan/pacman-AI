# Project 3: Reinforcement Learning

This project implements model-based and model-free reinforcement learning algorithms.

1. **Value Iteration Agent**: It utilizes an MDP and runs value iteration for set iterations before the constructor returns. It implements both asynchronous & prioritized sweeping.

2. **Q-Learning**: A RL agent that learns by trial and error from interactions with the environment through its update(state, action, nextState, reward) method. Approximate Q-learning is also implemented




### My solutions
- Eat points what make ghost scared first > eat ghosts
- Dont eat second copsule if scared > 0

##### Default result
> Pacman emerges victorious! Score: 1325 \
Average Score: 1352.4 \
Scores:        1346.0, 1549.0, 1320.0, 1340.0, 1320.0, 1322.0, 1321.0, 1343.0, 1338.0, 1325.0 \
Win Rate:      10/10 (1.00) \
Record:        Win, Win, Win, Win, Win, Win, Win, Win, Win, Win

##### Don't run away from ghosts if they are scared feature is implemented
> Average Score: 1595.5 \
Scores:        1747.0, 1335.0, 1347.0, 1937.0, 1919.0, 1727.0, 1533.0, 1330.0, 1540.0, 1540.0 \
Win Rate:      10/10 (1.00) \
Record:        Win, Win, Win, Win, Win, Win, Win, Win, Win, Win