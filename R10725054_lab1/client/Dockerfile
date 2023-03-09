# For more information, please refer to https://aka.ms/vscode-docker-python
FROM python:3.8-slim

# Turns off buffering for easier container logging
ENV PYTHONUNBUFFERED=1

ADD client.py /client/

# Install pip requirements
COPY requirements.txt .
RUN python -m pip install -r requirements.txt

WORKDIR /client/
