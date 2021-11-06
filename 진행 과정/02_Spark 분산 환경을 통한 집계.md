# Spark 분산 환경

`$ mkdir ~/adhoc`

`$ cd ~/adhoc`

- 콘솔 환경에서 수행

`$ export PYSPARK_DRIVER_PYTHON=jupyter-notebook`

- Spark를 기동하고 MongoDB용의 패키지 추가(2.2.0 - Spark Version)

`$ pyspark --packages org.mongodb.spark:mongo-spark-connector_2.11:2.2.0`

![image](https://user-images.githubusercontent.com/43158502/138860835-e624a3d3-1bba-4332-a043-f4bf504a9842.png)

> jupyter-notebook or jupyter-console 내에서 Pyspark 가동 

![image](https://user-images.githubusercontent.com/43158502/140610508-dfe5c7a3-07b3-4346-9de7-b7fbbe1d31ef.png)
> Pyspark와 MongoDB 연동하여 언어별 Tweet 확인

## Zeppelin 설치

- `Docker` 이용

`$ docker pull apache/zeppelin:0.8.2`
```
$ docker run -d --rm \
  -p 4040:8080 \
  -v $PWD/logs:/logs \
  -v $PWD/data:/data \
  -v $PWD/notebook:/notebook \
  -e ZEPPELIN_ADDR='0.0.0.0' \
  -e ZEPPELIN_NOTEBOOK_DIR='/notebook' \
  -e ZEPPELIN_LOG_DIR='/logs' \
  -- name zeppelin apache/zeppelin:0.8.2
```

![image](https://user-images.githubusercontent.com/43158502/138888174-f551a5f6-6b91-4ce9-8060-57c17beda06d.png)

![image](https://user-images.githubusercontent.com/43158502/138888757-9a864f75-a5c9-4256-bce1-f07461d2bccf.png)
> Zeppelin이 제대로 설치된 것을 확인할 수 있다.
