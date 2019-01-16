FROM jupyter/datascience-notebook:latest

RUN conda install --quiet --yes\
    'tensorflow' \
    'keras' && \
    conda clean -tipsy && \
    fix-permissions $CONDA_DIR && \
    fix-permissions /home/jovyan

RUN mkdir /home/jovyan/sources
WORKDIR /home/jovyan/sources
