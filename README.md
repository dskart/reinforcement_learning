# Reinforcement Learning

This repository contains the code for a Q-learning agent, which does very little on construction, but instead learns by trial and error from interactions with the environment through its update method. The agent aslo has access to epsilon-greedy actions. This agent is tested on a 2D grid world as well a pacman simulation.
This implementation was written without the use of any external library apart from Numpy.

This was made as an exercise to implement a reinforcement learning agent from scratch and run it on several different games. So please take in account that this code was written in a few days without any professional review/standard.

## Getting Started

This repository contains a lot of files. The only interesting file is ["qlearningAgents.py"](qlearningAgents.py) where the code for the Q learning agent is located.

### Prerequisites

- [Numpy](https://numpy.org/)

## Running the simulations

### Grid world

(with epsilon greedy random actions)

```[Python]
python3 gridworld.py -a q -k 100
```

### Bridge crossing

``` [Python]
python3 gridworld.py -a q -k 50 -n 0 -g BridgeGrid -e 1
```

Epsilon is controlled by -e, learning rate by -l.

### Pacman

```[python]
python3 pacman.py -p PacmanQAgent -x 2000 -n 2010 -l smallGrid
```

### Pacman with approximate Q-Learning

This works on bigger pacman grids compare to the classical Q-Learning agent

```[pyton]
python3 pacman.py -p ApproximateQAgent -a extractor=SimpleExtractor -x 50 -n 60 -l mediumClassic
```

## Authors

- **Raphael Van Hoffelen** - [github](https://github.com/dskart) - [website](https://www.raphaelvanhoffelen.com/)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
