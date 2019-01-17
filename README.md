# samples-basic-text-generation-lstm

deeply insipired by [Beginners Guide to Text Generation using LSTMs](https://www.kaggle.com/shivamb/beginners-guide-to-text-generation-using-lstms)

## Data Set

<https://www.kaggle.com/aashita/nyt-comments/version/13>

Unzip into text-generation-lstm/sources/data/nyt-comments folder.

## RUN DOCKER

This repository contains a basic docker-compose configuration to run a Jupyter Notebook server with Keras support (Tensor backend), using the default conda environment. This configuration automatically mounts the text-generation-lstm/sources folder inside the container, and sets it as the working directory.

```bash
docker-compose run
```

The notebook server can be accessed by navigating to <http://localhost:8900> on the host.

## RUN CONDA ENVIRONMENT

This repository contains a conda environment file in text-generation-lstm/sources folder.

Create environment:

```bash
conda env create -f environment.yml
```

Activate environment:

```bash
conda activate text-generation-lstm
```

Register new Kernel for Jupyter Notebook:

```bash
python -m ipykernel install --user --name text-generation-lstm --display-name "Python (text-generation-lstm)"
```

Run Jupyter Notebook Server:

```bash
jupyter notebook
```

Select "Python (text-generation-lstm)" from Kernel menu.

## TODO

* Containerized GPU support using [NVIDIA Container Runtime for Docker](https://github.com/NVIDIA/nvidia-docker). (Linux Only)
