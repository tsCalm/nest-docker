1. Dockerfile을 생성한다.

2. 도커 이미지를 빌드한다.

- docker build -t nest-docker .

3. 빌드된 도커 컨테이너 이미지를 실행한다.

- docker run -dp 3000:3000 nest-docker

4. 실행된 도커 컨테이너 이미지 상태를 확인한다.

- docker ps

5. 실행된 도커 컨테이너 이미지를 종료한다.

- docker kill CONTAINER_ID
