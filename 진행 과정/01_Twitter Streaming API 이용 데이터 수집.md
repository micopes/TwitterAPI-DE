## Twitter API 호출하는 Python 코드 작성
- Twitter Developers로부터
  - `consumer_key`
  - `consumer_secret`
  - `access_token_key`
  - `access_token_secret`
> 위의 key를 발급받았다.

- `import pymongo`
  - `sudo pip install pymongo` 를 통해 설치
- `import requests_oauthlib`
  - `python -m pip install --upgrade pip` 를 통해 pip upgrade 이후
  - `pip install requests_oauthlib` 를 통해 설치
- `import tqdm`
  - 왜인지 모르겠는데 `pip install tqdm`으로 설치도 되고 버전도 확인이 되었는데 모듈이 없다고 나온다.
  - `sudo apt install python3-tqdm`으로 설치를 추가로 했더니 된다.

### Twitter API 이용 수집 코드
![image](https://user-images.githubusercontent.com/43158502/138858847-ee4d5b57-917b-41b7-99d8-0fc2f0de6be1.png)

- 결과
![image](https://user-images.githubusercontent.com/43158502/138858479-2a967148-9b59-42c1-a00d-2c5ae532e5e5.png)

- 시험 삼아 약 5시간동안 약 1000000개의 데이터를 수집하여 MongoDB에 저장하였다.(이후에는 다른 Storage를 고려해야 한다. 열 지향 스토리지가 아니므로 고속 쿼리에는 적합하지 않다.)
