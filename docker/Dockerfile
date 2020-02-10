# base image
FROM continuumio/miniconda3:4.7.12

# set working directory
WORKDIR /usr/src/app

# install packages
COPY ./docker/environment.yml .
RUN conda update -n base conda && conda env update

# copy custom Jupyter Lab settings
COPY ./jupyter-codemirror-settings.json /root/.jupyter/lab/user-settings/@jupyterlab/codemirror-extension/commands.jupyterlab-settings

# run conda commands from environment
ENTRYPOINT ["conda", "run", "-n", "base"]
