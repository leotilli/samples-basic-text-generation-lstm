# samples-basic-text-generation-lstm

deeply insipired by [Beginners Guide to Text Generation using LSTMs](https://www.kaggle.com/shivamb/beginners-guide-to-text-generation-using-lstms)

## Data Set

<https://www.kaggle.com/aashita/nyt-comments/version/13>

Unzip into sources/data/nyt-comments folder.

## RUN

This repository contains a basic docker-compose configuration to run a Jupyter Notebook server with Keras support (Tensor backend), using the default conda environment. This configuration automatically mounts the text-generation-lstm/sources folder inside the container, and sets it as the working directory.

```bash
docker-compose run
```

The notebook server can be accessed by navigating to <http://localhost:8900> on the host.

## TODO

* Containerized GPU support using [NVIDIA Container Runtime for Docker](https://github.com/NVIDIA/nvidia-docker). (Linux Only)