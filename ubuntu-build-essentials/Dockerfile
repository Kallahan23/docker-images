# Ubuntu image with build-essential installed
# For compiling C and C++ programs
# Author: Danny K
#
# Usage: docker run -it -v $(pwd):/project/:rw kallahan23/ubuntu-build-essentials

FROM ubuntu:latest

RUN apt-get update && \
    apt-get install -y build-essential && \
    apt-get clean

RUN mkdir /project
WORKDIR /project

# Run bash when the container launches
CMD ["/bin/bash"]
