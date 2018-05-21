# Ubuntu image with build-essential installed
# For compiling C and C++ programs
#
# Usage: docker run -it -v $(pwd):/project/:rw ubuntu-build-essentials

FROM ubuntu:latest

RUN apt-get update && \
    apt-get install -y build-essential && \
    apt-get clean

RUN mkdir /project
WORKDIR /project

# Run bash when the container launches
CMD ["/bin/bash"]
