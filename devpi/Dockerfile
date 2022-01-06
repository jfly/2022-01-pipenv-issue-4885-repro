FROM python:3.8-buster

RUN pip install 'devpi-server==6.3.1'
RUN devpi-init

ENTRYPOINT ["devpi-server", "--host=0.0.0.0", "--port=3141"]
