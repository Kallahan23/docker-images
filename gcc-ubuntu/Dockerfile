# Ubuntu image with gcc and g++ installed
# For compiling C and C++ programs
#
# Usage: docker run -it -v /Project/Path/:/project/:rw cpp-ubuntu

FROM ubuntu:latest

RUN apt-get update && \
    apt-get install -y gcc g++

RUN mkdir /project
WORKDIR /project

# Run bash when the container launches
CMD ["/bin/bash"]
