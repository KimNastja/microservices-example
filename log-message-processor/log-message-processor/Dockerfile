FROM python:3.6-alpine

RUN apk add --no-cache build-base  \
    pip3 install -r requirements.txt
WORKDIR /usr/src/app
COPY requirements.txt .


COPY main.py .

CMD ["python3","-u","main.py"]

