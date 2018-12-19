# Centos image with Development Tools installed
# For compiling C and C++ programs
# Author: Danny K
#
# Usage: docker run -it -v $(pwd):/project/:rw kallahan23/centos-dev-tools

FROM centos:latest

RUN yum update -y && \
    yum groupinstall -y 'Development Tools' && \
    yum clean all && \
    rm -rf /var/cache/yum

RUN mkdir /project
WORKDIR /project

# Run bash when the container launches
CMD ["/bin/bash"]
