FROM python:3.8-buster

RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get install -y jq

WORKDIR /app
COPY Pipfile .
RUN pip install --upgrade pip

ARG JFLY_PIPENV_VERSION
RUN pip install "pipenv == $JFLY_PIPENV_VERSION"

ENTRYPOINT ["bash"]
