# Project: Reinforcement Learning

This project implements model-based and model-free reinforcement learning algorithms.

1. **Value Iteration Agent**: It utilizes an MDP and runs value iteration for set iterations before the constructor returns. It implements both asynchronous & prioritized sweeping.

2. **Q-Learning**: A RL agent that learns by trial and error from interactions with the environment through its update(state, action, nextState, reward) method. Approximate Q-learning is also implemented

### How to Run
- python pacman.py -p ApproximateQAgent -a extractor=myExtractor -x 50 -n 60 -l mediumClassic
- python pacman.py -p ApproximateQAgent -a extractor=myExtractor -x 50 -n 60 -l mediumGrid
- python pacman.py -p ApproximateQAgent -a extractor=myExtractor -x 50 -n 60 -l mylayout



##### Default result
> python pacman.py -p ApproximateQAgent -a extractor=SimpleExtractor -x 50 -n 60 -l mediumClassic
- Average Score: 1352.4 \
Scores:        1346.0, 1549.0, 1320.0, 1340.0, 1320.0, 1322.0, 1321.0, 1343.0, 1338.0, 1325.0 \
Win Rate:      10/10 (1.00) \
Record:        Win, Win, Win, Win, Win, Win, Win, Win, Win, Win

# Part 1
## Develop a sophisticated feature extractor
- Implemented feature: Don't run away from ghosts if they are scared.
> python pacman.py -p ApproximateQAgent -a extractor=myExtractor -x 50 -n 60 -l mediumClassic
- Average Score: 1595.5 \
Scores:        1747.0, 1335.0, 1347.0, 1937.0, 1919.0, 1727.0, 1533.0, 1330.0, 1540.0, 1540.0 \
Win Rate:      10/10 (1.00) \
Record:        Win, Win, Win, Win, Win, Win, Win, Win, Win, Win 

# Part 2
## Make a layout
mylayout.lay file is specifically designed to demonstrate the benefit of the sophisticated 
feature extractor which is developed for part 1. Thanks to the new feature extractor, 
the Pacman is able to eat all foods without running away from ghost and losing points redundantly.

> python pacman.py -p ApproximateQAgent -a extractor=SimpleExtractor -x 50 -n 60 -l mylayout 
- Average Score: 525.0 \
Scores:        529.0, 523.0, 528.0, 525.0, 521.0, 521.0, 528.0, 525.0, 525.0, 525.0 \
Win Rate:      10/10 (1.00) \
Record:        Win, Win, Win, Win, Win, Win, Win, Win, Win, Win 


> python pacman.py -p ApproximateQAgent -a extractor=myExtractor -x 50 -n 60 -l mylayout 
- Average Score: 778.0 \
Scores:        913.0, 763.0, 763.0, 763.0, 763.0, 763.0, 763.0, 763.0, 763.0, 763.0 \
Win Rate:      10/10 (1.00) \
Record:        Win, Win, Win, Win, Win, Win, Win, Win, Win, Win 
