# 전체 시스템을 실행 시키는 방법

## Front-end
> npm install
> 
> npm start

## Back-end
서버를 실행 코드
> uvicorn app.main:app --reload
>
특이사항: 처음 LLM모델을 불러올때는 다운로드를 받아야해서 조금 시간이 걸릴 수 있습니다. 그 이후에는 추론만 하면 질문이 생성됩니다.

## Docker Compose
> docker-compose up --build

docker-compose up --build 로 모든 컨테이너 실행.
로컬에서 테스트 및 디버깅 수행.


## 자동화 빌드 및 테스트 (GitHub Actions)
코드 변경 시, GitHub Actions가 자동으로 빌드 및 테스트 실행.
성공 시 Docker Hub에 최신 이미지 저장.

## 배포 (Kubernetes)
Kubernetes 클러스터에서 Docker 이미지를 사용하여 컨테이너 배포.
kubectl apply 명령으로 Deployment 및 Service 구성.
