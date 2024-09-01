# Use the official Jenkins agent image
FROM jenkins/agent:latest

# Switch to root user to install additional software
USER root

# Install Python 3 and pip
RUN apt-get update && \
    apt-get install -y python3 python3-pip && \
    rm -rf /var/lib/apt/lists/*

# Switch back to the Jenkins user
USER jenkins
