FROM ubuntu:latest

# Update ubuntu
RUN apt-get -y update

# Install software
RUN apt-get install -y git python python-setuptools python-dev build-essential

# Clone and install libais python library
RUN git clone https://github.com/schwehr/libais.git libais-repo
RUN cd libais-repo && python setup.py build && python setup.py install

