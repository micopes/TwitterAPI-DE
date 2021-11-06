# Twitter Streaming API를 이용 데이터 엔지니어링

#### 개발 전 세팅
- 시작
```
$ source schemaless-adhoc/bin/activate
$ sudo service mongodb start
```
- Zeppelin 실행
```
$ docker run -d --rm -p 4040:8080 -v $PWD/logs:/logs -v $PWD/data:/data -v $PWD/notebook:/notebook -e ZEPPELIN_ADDR='0.0.0.0' -e ZEPPELIN_NOTEBOOK_DIR='/notebook' -e ZEPPELIN_LOG_DIR='/logs' --name zeppelin apache/zeppelin:0.8.2
```

- Jupyter notebook 실행

`$ jupyter notebook`
