# Base Image selector
FROM ubuntu:latest

# Set Environment Variable
ENV DEBIAN_FRONTEND=noninteractive

RUN apt update -y && apt install fortune -y

ENTRYPOINT  /usr/games/fortune