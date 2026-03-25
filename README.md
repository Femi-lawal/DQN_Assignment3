# DQN_Assignment3

## Student Information

- Name: Oluwafemi Lawal
- Student ID: 8967308

## Assignment Summary

This repository contains CSCN8020 Assignment 3, which implements a Deep Q-Network (DQN) agent for the Pong Atari environment. The submission is organized around a single Jupyter notebook that:

- preprocesses Pong frames with the provided utility functions
- stacks four consecutive frames as the state representation
- implements the DQN algorithm in an object-oriented style
- trains and evaluates the agent
- reports score per episode and the moving average reward of the last five episodes
- compares the required batch-size and target-network update variations
- selects a best configuration based on the observed training results

## Repository Contents

- `CSCN8020_Assignment3.ipynb`: main notebook submission with markdown, code, plots, and conclusions
- `assignment3_utils.py`: provided preprocessing helper used by the notebook
- `requirements.txt`: Python dependencies for reproduction

## How To Run

1. Create and activate a Python environment.
2. Install the dependencies:

```bash
pip install -r requirements.txt
```

3. Open `CSCN8020_Assignment3.ipynb` in JupyterLab, Jupyter Notebook, or VS Code.
4. Run all cells from top to bottom.

The notebook will:

- train the experiments from scratch if no cached artifacts exist
- reuse saved artifacts from `artifacts/` if the experiment outputs are already present

## Notes

- The notebook first tries `PongDeterministic-v4` and falls back to the equivalent `ALE/Pong-v5` configuration if needed.
- Training Atari from pixels can take a while, so the notebook is easier to run on a machine with solid CPU or GPU resources.
