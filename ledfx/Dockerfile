## FROM jfloff
FROM jfloff/alpine-python:3.7

WORKDIR /src/

RUN apk update && \ 
 apk upgrade
RUN apk add portaudio-dev

COPY ./requirements.txt /requirements.txt

RUN pip install --upgrade pip
RUN pip install  -r /requirements.txt
RUN pip install ledfx
CMD ["ledfx"]

EXPOSE 8888    