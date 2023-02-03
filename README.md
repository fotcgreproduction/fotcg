# Codebase for the Reproduction of the paper *FOCUS ON THE COMMON GOOD: GROUP DISTRIBUTIONAL ROBUSTNESS FOLLOWS* by Piratla et al. (2022)

[View paper on Arxiv](https://arxiv.org/abs/2110.02619)

[Official Implementation on GitHub](https://github.com/vihari/CGD)

This repository contains the code used for the reproduction of the paper *FOCUS ON THE COMMON GOOD: GROUP DISTRIBUTIONAL ROBUSTNESS FOLLOWS* by Piratla et al. (2022).

## Requirements

the following `conda` environment was used: [fact3.yaml](fact3.yaml)

## Reproduction

The implementation of CGD we used is available [here](https://github.com/vihari/CGD).
The implementation of all algorithms and dataset pre-processing were integrated into the WILDS codebase ([version 1.2.2](https://github.com/p-lambda/wilds/releases/tag/v1.2.2)). For the sake of completeness and to make re-running our experiments as easy as possible, we provide here all required files to reproduce our experiments. Furthermore, we include the `.job` files used to run the experiments using the SLURM scheduler.

### Detailed Instructions for Reproduction

1. install the `conda` environment from the provided [fact3.yaml](fact3.yaml) file using e.g. `conda create -n fact --file fact3.yaml`
2. set up wandb
3. the notebook handles all instructions needed to reproduce the experiments

#### Setting up wandb

see also the reference [here](https://docs.wandb.ai/quickstart).

1. create a wandb account, if not already done
2. install wandb: using `pip install wandb`, if not already done
3. in the console, login to wandb: `wandb login` and provide your wandb API key, which can be found in your account settings. From now on, wandb will be configured to use your account.
4. We advice to select the option to store the API key locally, so that you do not have to login every time you want to start an experiment. Our jobfiles are configured to use wandb for logging, and to store the results of the experiments.

## Evaluation

Follows standard WILDS protocoll and metrics provided there.

## Results

All our results can be found in the report, and the official results are available here: [WILDS Leaderboard](https://wilds.stanford.edu/leaderboard/).
