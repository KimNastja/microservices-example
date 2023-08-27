FROM python:3.6-alpine

WORKDIR /usr/src/app
RUN apk add --no-cache build-base  \
    pip3 install -r requirements.txt
    
COPY requirements.txt .

COPY main.py .

CMD ["python3","-u","main.py"]

