# Ubuntu image with gcc and g++ installed
# For compiling C and C++ programs
#
# Usage: docker run -it -v $(pwd):/project/:rw gcc-ubuntu

FROM ubuntu:latest

RUN apt-get update && \
    apt-get install -y build-essential

RUN mkdir /project
WORKDIR /project

# Run bash when the container launches
CMD ["/bin/bash"]
