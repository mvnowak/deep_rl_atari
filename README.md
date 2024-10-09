# Reinforcement-Learning-Atari

DQN Implementation for Atari games from the [MinAtar](https://github.com/kenjyoung/MinAtar) library.

## Introduction

This repository contains a framework for the Deep Learning DQN algorithm with the following extensions:

- [x] Double DQN
- [x] Prioritized Experience Replay
- [x] Dueling DQN
- [x] Noisy DQN


## Installation

To install the required packages, run the following command:

```bash
pip install -r requirements.txt
```

## Training

Training parameters are fully documented in the CLI client. Run the following command to see all the available options:

```bash
python scripts/cli.py train --help
```

to revise all possible parameters.

### Training from config file

To train an agent from a config file, run the following command:

```bash
python scripts/cli.py train -f <path-to-config-file>
```

An example config file is provided as `config.yaml`.


## Live Mode

To run the agent in live mode, run the following command:

```bash
python scripts/cli.py live --help
```

or 

```bash
python scripts/cli.py minatar-live --help
```

for MinAtar environments.

## Live Demo

```bash
python scripts/cli.py minatar-live --checkpoint_path data/Breakout/mini_rainbow/03/checkpoints/epoch=9999-step=20000.ckpt
```

```bash
python scripts/cli.py minatar-live --checkpoint_path data/Freeway/mini_rainbow/03/checkpoints/epoch=9999-step=20000.ckpt
```

```bash
python scripts/cli.py minatar-live --checkpoint_path logs/MinAtar_SpaceInvaders/version_0/checkpoints/epoch=49999-step=100000.ckpt
```

