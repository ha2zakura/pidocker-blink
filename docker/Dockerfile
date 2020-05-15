FROM balenalib/rpi-raspbian:buster

RUN apt-get update && apt-get install -y \
  build-essential \
  python3-dev \
  python3-distutils \
  && rm -rf /var/lib/apt/lists/*

RUN curl https://bootstrap.pypa.io/get-pip.py -k -o get-pip.py && \
  python3 get-pip.py

RUN pip install rpi.gpio
