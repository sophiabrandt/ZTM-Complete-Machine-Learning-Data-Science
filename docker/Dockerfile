# base image
FROM continuumio/miniconda3:4.7.12

# set working directory
WORKDIR /usr/src/app

# install packages
COPY ./docker/environment.yml .
RUN conda update -n base conda && conda env update
