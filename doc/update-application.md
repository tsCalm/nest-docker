## 테스트 과정

1. 내부 코드를 업데이트한다.

2. 도커 컨테이너 이미지를 다시 빌드한다.

3. 실행중인 도커 컨테이너를 중지시킨다.

4. 빌드한 도커 컨테이너 이미지를 다시 실행한다.

## 궁금증

- 이미 실행중인 도커 컨테이너 이미지의 태그 이름이 같은 경우 hot-reload되지 않을까?

빌드 및 실행을 해줘야함.. 그것도 실행중인 도커 컨테이너 이미지를 종료한 후 실행해야 한다.

도커 이미지를 실행중 같은 태그의 이미지를 실행시키면 아래와 같은 에러 발생

```
docker: Error response from daemon: driver failed programming external connectivity on endpoint interesting_margulis (492cc7584851d0b93734a00443ab3f14fa1191aec5e1ba140f41d837b5a4c1): Bind for 0.0.0.0:3000 failed: port is already allocated.
```
