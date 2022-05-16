FROM jupyter/datascience-notebook:python-3.9.12
USER root

# Update
RUN apt-get update && apt-get -y upgrade

RUN pip install -U pip poetry

COPY pyproject.toml poetry.lock ./

RUN poetry config virtualenvs.create false && \
    poetry install --no-interaction
