# Spark 분산 환경

`$ mkdir ~/adhoc`

`$ cd ~/adhoc`

- 콘솔 환경에서 수행

`$ export PYSPARK_DRIVER_PYTHON=jupyter-console`

- Spark를 기동하고 MongoDB용의 패키지 추가(3.1.1 - Spark Version)

`$ pyspark --packages org.mongodb.spark:mongo-spark-connector_2.11:3.1.1`

![image](https://user-images.githubusercontent.com/43158502/138860835-e624a3d3-1bba-4332-a043-f4bf504a9842.png)

> jupyter-console 내에서 Pyspark 가동 

## Zeppelin 설치

`$ wget https://downloads.apache.org/zeppelin/zeppelin-0.9.0-preview2/zeppelin-0.9.0-preview2-bin-all.tgz`
