# Use an official Python runtime as a parent image
FROM ubuntu:latest

# Make port 80 available to the world outside this container
EXPOSE 80

# RUN add-apt-repository ppa:kivy-team/kivy
RUN apt-get update
RUN apt-get install -y python3
RUN apt-get install -y python3-kivy

# Run app.py when the container launches
CMD ["python3"]
