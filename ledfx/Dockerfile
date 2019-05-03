## FROM jfloff
FROM jfloff/alpine-python:3.7

WORKDIR /src/

RUN apk update
RUN apk upgrade
# RUN apt install python3 python3-pip -y 

COPY ./requirements.txt /requirements.txt

RUN pip install --upgrade pip
RUN pip install  -r /requirements.txt
RUN pip install ledfx

CMD ["/bin/bash"]
    