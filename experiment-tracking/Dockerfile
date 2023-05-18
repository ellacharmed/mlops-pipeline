FROM python:3.11-slim-buster

RUN pip install mlflow boto3 pymysql minio scikit-learn cryptography

WORKDIR /training
COPY ./tests.py .
COPY ./kc_house_data.csv .
COPY ./train.py .
