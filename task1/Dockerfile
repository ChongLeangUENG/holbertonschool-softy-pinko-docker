FROM ubuntu:latest

RUN apt-get update && apt-get upgrade -y

RUN apt-get install -y python3 python3-pip && \
    rm /usr/lib/python*/EXTERNALLY-MANAGED

RUN pip3 install Flask

WORKDIR /app

COPY api.py /app

EXPOSE 5252

CMD ["python3", "api.py"]
