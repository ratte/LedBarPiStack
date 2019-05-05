## Install ledFx into RaspberryPi Compatible Docker
## 

FROM jfloff/alpine-python:3.7

RUN apk update && apk upgrade
RUN apk add portaudio-dev

COPY ./requirements.txt /requirements.txt
COPY ./config/config.yaml /root/.ledfx/config.yaml

RUN pip install --upgrade pip
RUN pip install  -r /requirements.txt
RUN pip install ledfx

# run it
CMD ["/bin/bash","ledfx"]

# Port which is exposed
EXPOSE 8888  