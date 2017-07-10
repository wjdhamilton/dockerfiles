# Use FPComplete's ubuntu base for Haskell runtimes
FROM fpco/ubuntu-with-libgmp:latest

RUN apt-get update && apt-get install -y \
  curl \
  software-properties-common


RUN curl -sSL https://get.haskellstack.org/ | sh
  
RUN export PATH=$PATH:/usr/local/bin

# Add the haskell executable

RUN stack setup 
