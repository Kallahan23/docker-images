# Centos image with gcc and g++ installed
# For compiling C and C++ programs
#
# Usage: docker run -it -v $(pwd):/project/:rw gcc-centos

FROM centos:latest

RUN yum update && \
    yum groupinstall -y 'Development Tools'

RUN mkdir /project
WORKDIR /project

# Run bash when the container launches
CMD ["/bin/bash"]
