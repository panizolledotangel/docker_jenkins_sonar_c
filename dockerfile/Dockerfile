FROM jenkins/jenkins:lts

# Switch to the root user
USER root

# Install build-essential and cmake
RUN apt-get update && \
    apt-get install -y build-essential cmake
    
RUN apt-get install wget
RUN apt-get install unzip

RUN wget http://sonarcloud.io/static/cpp/build-wrapper-linux-x86.zip 
RUN unzip build-wrapper-linux-x86.zip
RUN mv build-wrapper-linux-x86 /opt/

# Switch back to the jenkins user
USER jenkins
