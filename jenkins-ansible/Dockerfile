FROM jenkinsci/blueocean

USER root

RUN apk add python python3 python3-dev
RUN apk add build-base mpc1-dev libressl-dev libffi-dev
RUN apk add sshpass
RUN apk add nano

RUN curl -O https://bootstrap.pypa.io/get-pip.py && \
    python3 get-pip.py && \
    pip3 install ansible --upgrade && \
    pip3 install awscli --upgrade

USER jenkins
