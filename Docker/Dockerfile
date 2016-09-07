# FROM ubuntu:latest
FROM gcr.io/tensorflow/tensorflow

# Update ubuntu
RUN apt-get -y update

# Install software
RUN apt-get install -y git python python-setuptools python-dev build-essential python-pip

# Clone and install libais python library
RUN git clone https://github.com/schwehr/libais.git libais-repo
RUN cd libais-repo && python setup.py build && python setup.py install

# Settings and prefs
RUN echo "alias ls=\"ls -laG\"" >> ~/.bashrc

