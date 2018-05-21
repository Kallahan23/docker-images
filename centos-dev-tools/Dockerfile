# Centos image with Development Tools installed
# For compiling C and C++ programs
#
# Usage: docker run -it -v $(pwd):/project/:rw centos-dev-tools

FROM centos:latest

RUN yum update && \
    yum groupinstall -y 'Development Tools' && \
    yum clean all && \
    rm -rf /var/cache/yum

RUN mkdir /project
WORKDIR /project

# Run bash when the container launches
CMD ["/bin/bash"]
