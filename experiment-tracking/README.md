## To Run
```
    docker-compose --env-file ./.env up
    docker exec -it mlflow_server bash
```


```docker run -p 9000:9000 -p 9001:9001 --name minio -d -v ~/minio/data:/data -e "MINIO_ROOT_USER={MINIO_ROOT_USER}" -e "MINIO_ROOT_PASSWORD={MINIO_ROOT_PASSWORD}" minio/minio server --console-address :9001 /data```

```cp experiment-tracking/buckets/mlflow/1/20a1d7ed33164ddc962235fe48f42f33/artifacts/rf-regressor/model.pkl ml-app```
