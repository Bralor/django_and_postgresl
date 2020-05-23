FROM python:3.8.0-alpine

WORKDIR /usr/src/e_auctions

# Prevent Python to create .pyc files
ENV PYTHONDONTWRITEBYTECODE 1
# Prevent Python to buffering stdout sterr
ENV PYTHONUNBUFFERED 1

RUN pip install --upgrade pip
COPY ./requirements.txt /usr/src/e_auctions/requirements.txt
RUN pip install -r requirements.txt

COPY . /usr/src/e_auctions/
