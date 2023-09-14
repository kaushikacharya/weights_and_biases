# Weights & Biases 101

## Course info

- [Course url](https://www.wandb.courses/courses/wandb-101)
- [code repository](https://github.com/wandb/edu/tree/main/wandb101)

## Course contents

1. [Introducing W & B](#introducing-w--b)
2. [Instrumenting W&B in your code](#instrumenting-wb-in-your-code)
3. [Exploring W&B workspace](#exploring-wb-workspace)
4. [Comparing & analyzing experiments](#comparing--analyzing-experiments)
5. [Using W&B beyond experiment tracking](#using-wb-beyond-experiment-tracking)
6. Testing your knowledge
7. [Logging your first run](#logging-your-first-run)
8. [More resources for you](#more-resources-for-you)

### Introducing W & B

- This lesson introduces Weights & Biases (W&B)
  - An MLOps platform to track and organize machine learning experiments.
- Explains how W&B can be integrated to log metrics and configurations for easy tracking and visualization.
  - Demonstrated using a PyTorch training script.

### Instrumenting W&B in your code

- Demonstrates how to install and integrate W&B Python client into training script.
- Shows how to refactor code to create a run, gather configurations and pass them to ```wandb.init()```.
- ```wandb.log()``` to store and visualize the history of each metric throughout the training process.

### Exploring W&B workspace

- Instructor demonstrates
  - How to run a training script integrated with Weights & Biases - Navigate the W&B workspace to view real-time metrics, interact with plots, and access system metrics.
  - Highlights W&B's ability to capture information that helps with reproducibility.

### Comparing & analyzing experiments

- Proper way of finishing W&B run:
  - Python script:
    - Finishes as and when script run is over.
  - Notebook:
    - ```wandb.finish()``` or
    - Context manager

### Using W&B beyond experiment tracking

- Covers the advanced features of the Weights & Biases platform.
  - [Sweeps](https://docs.wandb.ai/guides/sweeps)
    - Hyperparameter optimization
  - [Tables](https://docs.wandb.ai/guides/data-vis/tables-quickstart)
    - Data visualization and evaluation
  - [Artifacts](https://docs.wandb.ai/guides/artifacts/)
    - Data lineage tracking
  - Models
    - Storing and reproducing model development
  - [Reports](https://docs.wandb.ai/guides/reports)
    - Sharing key metrics and analysis with stakeholders.

### Testing your knowledge

### Logging your first run

- [Example dashboard](https://wandb.ai/wandb/wandb_example)
- [User settings](https://wandb.ai/settings)
- Colab Notebooks
  - [Intro to Weights & Biases](https://colab.research.google.com/github/wandb/examples/blob/master/colabs/intro/Intro_to_Weights_%26_Biases.ipynb)
  - [Hyperparameters sweeps using PyTorch](https://colab.research.google.com/github/wandb/examples/blob/master/colabs/pytorch/Organizing_Hyperparameter_Sweeps_in_PyTorch_with_W%26B.ipynb)

### More resources for you

- [W&B Fully Connected](https://wandb.ai/fully-connected)
  - Blog on ML and MLOps knowledge
- [W&B Docs](https://docs.wandb.ai/)
- [W&B community](https://wandb.me/discord)
- [Youtube: Tune Hyperparameters Easily with W&B Sweeps](https://www.youtube.com/watch?v=9zrmUIlScdY&list=PLD80i8An1OEGajeVo15ohAQYF1Ttle0lk)
- [W&B Server](https://docs.wandb.ai/guides/hosting)
  - [Basic Setup](https://docs.wandb.ai/guides/hosting/how-to-guides/basic-setup) describes steps to host locally.

## Assignments

|Assignment|Description|
|----------|-----------|
|[Intro to W&B](https://colab.research.google.com/drive/1GqU8SKVFiZwFWAIqepG_FDjXpS7r9ZqS)| 1. Run an experiment by passing hyperparameters. 2. Log metrics.  3. Visualize results in dashboard.|
