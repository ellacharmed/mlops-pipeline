FROM python:3.11

WORKDIR /app
COPY ./requirements.txt /app
RUN pip install -r requirements.txt

COPY . /app

EXPOSE 5000
ENV MODEL_NAME Model
ENV SERVICE_TYPE MODEL
ENV PERSISTANCE 0

CMD exec seldon-core-microservice ${MODEL_NAME} --service-type ${SERVICE_TYPE}