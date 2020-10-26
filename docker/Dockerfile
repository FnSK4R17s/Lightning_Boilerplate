FROM pytorch/pytorch:1.6.0-cuda10.1-cudnn7-runtime

# run in apt-get update for sanity
RUN apt-get update \
    && apt-get upgrade -y \
    && apt-get install -y wget zip git \
    && apt install unzip \
    && python3 -m pip install --upgrade pip

COPY requirements.txt requirements.txt

RUN pip install -r requirements.txt