# Use an official Python runtime as a parent image
FROM ubuntu:latest

# RUN add-apt-repository ppa:kivy-team/kivy
RUN apt-get update && \
    apt-get install -y gcc g++

RUN mkdir /project
WORKDIR /project

# Run app.py when the container launches
CMD ["/bin/bash"]
