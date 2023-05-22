# Dockerfile

# Author       : MR.KK
# Github       : https://github.com/MR.KK
# Messenger    : https://m.me/MR.KK
# Email        : maramkarthik21@gmail.com
# Date         : 08-09-2022
# Main Language: Python

# Download and import main images

# Operating system
FROM debian:latest
# Main package
FROM python:3

# Author info
LABEL MAINTAINER="https://github.com/MR.KK/MaxPhisher"

# Working directory
WORKDIR MaxPhisher/
# Add files 
ADD . /MaxPhisher

# Installing other packages
RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install php openssh-client -y
RUN pip3 install -r files/requirements.txt
RUN apt-get clean

# Main command
CMD ["python3", "maxphisher.py", "--noupdate"]

## Wanna run it own? Try following commnads:

## "sudo docker build . -t MR.KK/maxphisher:latest", "sudo docker run --rm -it MR.KK/maxphisher:latest"

## "sudo docker pull MR.KK/maxphisher", "sudo docker run --rm -it MR.KK/maxphisher"
