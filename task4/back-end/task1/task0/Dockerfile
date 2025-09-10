FROM ubuntu:latest

RUN apt-get update && apt-get upgrade -y && \
    apt-get install -y python3 python3-pip && \
    rm -rf /var/lib/apt/lists/*

RUN pip3 install --no-cache-dir flask

WORKDIR /app
COPY ./api.py /app/api.py

CMD ["python3", "api.py"]
