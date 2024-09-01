FROM ubuntu:latest

RUN apt-get update

RUN apt-get upgrade -y

RUN apt-get install python3-pip -y

RUN apt-get install python3 -y

RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

RUN pip3 install flask

WORKDIR /app

COPY api.py /app/

EXPOSE 5252

CMD ["python3", "api.py"]
