# Ubuntu image with python3-kivy installed

FROM ubuntu:latest

# RUN add-apt-repository ppa:kivy-team/kivy
RUN apt-get update && \
    apt-get install -y python3 python3-kivy

RUN mkdir /project
WORKDIR /project

# Run python3 when the container launches
CMD ["python3"]
