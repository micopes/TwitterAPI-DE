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
`<...>`
