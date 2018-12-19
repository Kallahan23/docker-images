# Author: Danny K

FROM ubuntu:latest

RUN apt-get update && \
    apt-get install -y nodejs && \
    apt-get install -y npm && \
    npm install -g create-react-native-app

# Run bash when the container launches
CMD ["/bin/bash"]
